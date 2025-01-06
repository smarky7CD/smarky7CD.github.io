---
title: "Research"
description: "A list of my publications."
---

Paper PDFs can be found by clicking on the title. 


Various author ordering conventions used. 

## Peer-reviewed publications

--- 

#### 2024

--- 

### [Leveraging Generative Models for Covert Messaging: Challenges and Tradeoffs for "Dead-Drop" Deployments](/bhmbs24.pdf) 

Luke A Bauer, James K. Howes, **Sam A. Markelon**, Vincent Bindschaedler, and Thomas Shrimpton

[CODASPY '24](https://dl.acm.org/doi/abs/10.1145/3626232.3653264)

<details>

<summary>Abstract</summary>

<br>

<p>State of the art generative models of human-produced content are the focus of many recent papers that explore their use for steganographic communication. In particular, generative models of natural language text. Loosely, these works (invertibly) encode message-carrying bits into a sequence of samples from the model, ultimately yielding a plausible natural language covertext. By focusing on this narrow steganographic piece, prior work has largely ignored the significant algorithmic challenges, and performance-security tradeoffs, that arise when one actually tries to build a messaging pipeline around it. We make these challenges concrete, by considering the natural application of such a pipeline: namely, "dead-drop" covert messaging over large, public internet platforms (e.g. social media sites). We explicate the challenges and describe approaches to overcome them, surfacing in the process important performance and security tradeoffs that must be carefully tuned. We implement a system around this model-based format-transforming encryption pipeline, and give an empirical analysis of its performance and (heuristic) security.</p>
</details>

<details>
<summary>Citation</summary>

```
@inproceedings{bhmbs24,
    title={Leveraging Generative Models for Covert Messaging: Challenges and Tradeoffs for" Dead-Drop" Deployments},
    author={Bauer, Luke A and Howes, James K and Markelon, Sam A and Bindschaedler, Vincent and Shrimpton, Thomas},
    booktitle={Proceedings of the Fourteenth ACM Conference on Data and Application Security and Privacy},
    pages={67--78},
    year={2024} 
}
```

</details>

---

#### 2023

---

### [Compact Frequency Estimators in Adversarial Environments](/mfs23.pdf) 

**Sam A. Markelon**, Mia Filić, and Thomas Shrimpton

[CCS '23](https://dl.acm.org/doi/abs/10.1145/3576915.3623216)

<details>

<summary>Abstract</summary>

<br>

<p>Count-Min Sketch (CMS) and HeavyKeeper (HK) are two realizations of a compact frequency estimator (CFE). These are a class of probabilistic data structures that maintain a compact summary of (typically) high-volume streaming data, and provides approximately correct estimates of the number of times any particular element has appeared. CFEs are often the base structure in systems looking for the highest-frequency elements (i.e., top-K elements, heavy hitters, elephant flows). Traditionally, probabilistic guarantees on the accuracy of frequency estimates are proved under the implicit assumption that stream elements do not depend upon the internal randomness of the structure. Said another way, they are proved in the presence of data streams that are created by non-adaptive adversaries. Yet in many practical use-cases, this assumption is not well-matched with reality; especially, in applications where malicious actors are incentivized to manipulate the data stream. We show that the CMS and HK structures can be forced to make significant estimation errors, by concrete attacks that exploit adaptivity. We analyze these attacks analytically and experimentally, with tight agreement between the two. Sadly, these negative results seem unavoidable for (at least) sketch-based CFEs with parameters that are reasonable in practice. On the positive side, we give a new CFE (Count-Keeper) that can be seen as a composition of the CMS and HK structures. Count-Keeper estimates are typically more accurate (by at least a factor of two) than CMS for "honest" streams; our attacks against CMS and HK are less effective (and more resource intensive) when used against Count-Keeper; and Count-Keeper has a native ability to flag estimates that are suspicious, which neither CMS or HK (or any other CFE, to our knowledge) admits.</p>
</details>

<details>
<summary>Citation</summary>

```
@inproceedings{mfs23,
    title={Compact Frequency Estimators in Adversarial Environments},
    author={Markelon, Sam A and Filic, Mia and Shrimpton, Thomas},
    booktitle={Proceedings of the 2023 ACM SIGSAC Conference on Computer and Communications Security},
    pages={3254--3268},
    year={2023}
}
```

</details>

---

#### 2022

---

### [The DecCert PKI: A Solution to Decentralized Identity Attestation and Zooko’s Triangle](/mt22.pdf) 

**Sam A. Markelon** and John True

[DAPPS '22](https://ieeexplore.ieee.org/abstract/document/9899851)

<details>

<summary>Abstract</summary>

<br>

<p>We propose DecCert, a decentralized public key infrastructure designed as a smart contract that solves the problem of identity attestation on public blockchains. Our system allows an individual to bind an identity to a public blockchain address. Once a claim of identity is made by an individual, other users can choose to verify the attested identity based on the evidence presented by an identity claim maker by staking cryptocurrency in the DecCert smart contract. Increasing levels of trust are naturally built based upon the amount staked and the duration the collateral is staked for. This mechanism replaces the usual utilization of digital signatures in a traditional hierarchical certificate authority model or the web of trust model to form a publicly verifiable decentralized stake of trust model. We also present a novel solution to the certificate revocation problem and implement our solution on the Ethereum blockchain. Further, we show that our design solves Zooko’s triangle as defined for public key infrastructure deployments.</p>
</details>

<details>
<summary>Citation</summary>

```
@inproceedings{mt22,
    title={The DecCert PKI: A Solution to Decentralized Identity Attestation and Zooko’s Triangle},
    author={Markelon, Sam A and True, John},
    booktitle={2022 IEEE International Conference on Decentralized Applications and Infrastructures (DAPPS)},
    pages={74--82},
    year={2022},
    organization={IEEE}
} 
```

</details>

---

#### 2020

---

### [A semi-quantum extended B92 protocol and its analysis](/km20.pdf) 

Walter O. Krawec and **Sam A. Markelon**

[Quantum Information Science, Sensing, and Computation XII](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11391/113910G/A-semi-quantum-extended-B92-protocol-and-its-analysis/10.1117/12.2558200.short)

<details>

<summary>Abstract</summary>

<br>

<p>Unlike purely classical communication, unconditionally secure key distribution is possible if Alice and Bob are both equipped with quantum hardware. The degree to which a protocol needs to be quantum is not only an interesting theoretical question, but also important for practical implementations. Indeed, one may wish to construct cheaper devices, or compensate for device malfunction. In this sense, studying limited resource QKD protocols is an important problem. One direction to studying this is the semi-quantum model introduced by Boyer et al. in 2007 (PRL 99 140501). Several provably secure semi-quantum protocols were put forth. However, most of these protocols were proven secure in the perfect qubit scenario and not necessarily against practical attacks. Only recently, starting with seminal work of Boyer, Katz, Liss, and Mor in (PRA 96 062335) has research in the field of semi-quantum cryptography considered practical devices and imperfections, such as multi photon sources and imperfect detectors. In this work, we present a new SQKD protocol based on an Extended B92 protocol which is able to counter certain practical attacks. Furthermore, the techniques we use may see broad application to other limited-resource (S)QKD protocols.</p>
</details>

<details>
<summary>Citation</summary>

```
@inproceedings{km20,
    title={A semi-quantum extended B92 protocol and its analysis},
    author={Krawec, Walter O and Markelon, Sam A},
    booktitle={Quantum Information Science, Sensing, and Computation XII},
    volume={11391},
    pages={47--55},
    year={2020},
    organization={SPIE}
}
```

</details>

---

#### 2018

---

### [Genetic algorithm to study practical quantum adversaries](/km18.pdf) 

Walter O. Krawec and **Sam A. Markelon**

[GECCO '18](https://dl.acm.org/doi/abs/10.1145/3205455.3205478)

<details>

<summary>Abstract</summary>

<br>

<p>In this paper we show how genetic algorithms can be effectively applied to study the security of arbitrary quantum key distribution (QKD) protocols when faced with adversaries limited to current-day technology. We compare two approaches, both of which take into account practical limitations on the quantum power of an adversary (which can be specified by the user). Our system can be used to determine upper-bounds on noise tolerances of novel QKD protocols in this scenario, thus making it a useful tool for researchers. We compare our algorithm's results with current known numerical results, and also evaluate it on newer, more complex, protocols where no results are currently known.</p>
</details>

<details>
<summary>Citation</summary>

```
@inproceedings{km18,
    title={Genetic algorithm to study practical quantum adversaries},
    author={Krawec, Walter O and Markelon, Sam A},
    booktitle={Proceedings of the Genetic and Evolutionary Computation Conference},
    pages={1270--1277},
    year={2018}
}
```

</details>

---

## Pre-prints

--- 

#### 2024

--- 

### [A Formal Treatment of Key Transparency Systems with Scalability Improvements](/bfm24.pdf) 

Nicholas Brandt, Mia Filić, and  **Sam A. Markelon**

<details>

<summary>Abstract</summary>

<br>

<p>Key Transparency (KT) systems have emerged as a critical technology for securely distributing and verifying the correctness of public keys used in end-to-end encrypted messaging services. Despite substantial academic interest, increased industry adoption, and IETF standardization efforts, KT systems lack a holistic and formalized security model, limiting their resilience to practical threats and constraining future development. In this paper, we introduce the first cryptographically sound formalization of KT as an ideal functionality, clarifying the assumptions, security properties, and potential vulnerabilities of deployed KT systems. We identify a significant security concern — a possible impersonation attack by a malicious service provider — and propose a backward-compatible solution. Additionally, we address a core scalability bottleneck by designing and implementing a novel, privacy-preserving verifiable Bloom filter (VBF) that significantly improves KT efficiency without compromising security. Experimental results demonstrate the effectiveness of our approach, marking a step forward in both the theoretical and practical deployment of scalable KT solutions.</p>
</details>

<details>
<summary>Citation</summary>

```
@misc{bfm24,
    author = {Nicholas Brandt and Mia Filić and Sam A. Markelon},
    title = {A Formal Treatment of Key Transparency Systems with Scalability Improvements},
    howpublished = {Cryptology {ePrint} Archive, Paper 2024/1938},
    year = {2024},
    url = {https://eprint.iacr.org/2024/1938}
}
```

</details>

---

### [Probabilistic Data Structures in the Wild: A Security Analysis of Redis](/fhmpu24.pdf) 

Mia Filić, Jonas Hofmann, **Sam A. Markelon**, Kenneth G Paterson, and  Anupama Unnikrishnan

<details>

<summary>Abstract</summary>

<br>

<p>
Redis (Remote Dictionary Server) is a general purpose, in-memory database that supports a rich array of functionality, including various Probabilistic Data Structures (PDS), such as Bloom filters, Cuckoo filters, as well as cardinality and frequency estimators. These PDS typically perform well in the average case. However, given that Redis is intended to be used across a diverse array of applications, it is crucial to evaluate how these PDS perform under worst-case scenarios, ie, when faced with adversarial inputs. We offer a comprehensive analysis to address this question. We begin by carefully documenting the different PDS implementations in Redis, explaining how they deviate from those PDS as described in the literature. Then we show that these deviations enable a total of 10 novel attacks that are more severe than the corresponding attacks for generic versions of the PDS. We highlight the critical role of Redis' decision to use non-cryptographic hash functions in the severity of these attacks. We conclude by discussing countermeasures to the attacks, or explaining why, in some cases, countermeasures are not possible.</p>
</details>

<details>
<summary>Citation</summary>

```
@misc{fhmpu24,
    author = {Mia Filić and Jonas Hofmann and Sam A. Markelon and Kenneth G. Paterson and Anupama Unnikrishnan},
    title = {Probabilistic Data Structures in the Wild: A Security Analysis of Redis},
    howpublished = {Cryptology {ePrint} Archive, Paper 2024/1312},
    year = {2024},
    url = {https://eprint.iacr.org/2024/1312}
}
```

</details>

---