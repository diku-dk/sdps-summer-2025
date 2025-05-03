# SDPS Summer Rehearsal 2025

On Wednesday, May 14 there will be an event in which everybody interested and willing will practice their chosen forthcoming PhD defense, summer-conference presentation, or any other talk for which feedback and practice is desirable. For confirmed attendees, lunch will be provided.

### Location:
The event will take place at SCI-DIKU-UP1-1-1-N116A. 

### Programme:

**Talk 1**: *vMODB: Unifying event and data management for distributed asynchronous applications*

**Speaker:** Rodrigo Laigner

<details><summary><b>Abstract</b></summary>
Event-driven architecture (EDA) has emerged as a crucial architectural pattern for scalable cloud applications. However, its asynchronous and decoupled nature introduces challenges in meeting transactional requirements. Database systems, relegated to serving as storage engines for individual components, do not recognize transactions that span multiple components in EDAs. In contrast, messaging systems are unaware of the components' application states. Weaving such asynchronous and independent EDA components forces developers to relinquish transactional guarantees, resulting in data consistency issues.
To address this challenge, we design vMODB, a distributed framework that enables the implementation of highly consistent and scalable cloud applications without compromising the envisioned benefits of EDA. We propose Virtual Micro Service (VMS), a novel programming model that provides familiar constructs to enable developers to specify the data model, constraints, and concurrency semantics of components, as well as transactions and data dependencies that span across components. vMODB leverages VMS semantics to enforce ACID properties by transparently unifying event logs and state management into a common event-driven execution framework. Our experiments using two benchmarks show that vMODB outperforms a widely adopted state-of-the-art competing framework that only offers eventual consistency by up to 3X. With its high performance, familiar programming constructs, and ACID properties, vMODB will significantly simplify the development of highly consistent and efficient EDAs.
</details>

<details><summary><b>Bio</b></summary>
Rodrigo Laigner is soon defending his PhD at University of Copenhagen and is now a Postdoc at SDPS section. His research targets devising effective programming abstractions and efficient systems for emerging data-intensive applications. During his doctoral studies, he published relevant articles about distributed data-intensive applications in the cloud.
</details>

<p>&nbsp;</p>

**Talk 2:** *PILOS: Scalable Large-Subgraph Matching by Online Spectral Filtering*

**Speaker:** Konstantinos Skitsas

<details><summary><b>Abstract</b></summary>
Subgraph matching seeks all the occurrences of a query graph inside another graph. As it reduces to subgraph isomorphism, it is NP-hard. Current methods reduce the computation by filtering the candidates on which they run subgraph isomorphism. Nevertheless, when the query is large, the number of candidates grows rapidly, rendering current methods largely ineffective in pruning and incapable to answer even within one hour. A primary reason for this ineffectiveness is their inability to effectively consider the query graph structure in the computation. In this paper, we propose PILOS, a novel matching algorithm that substantially improves the filtering phase of a typical matching algorithm and computes up to 60% fewer candidates for verification. PILOS uses (i) an offline light-weight index-based phase, which leverages the top graph Laplacian eigenvalues of query and data node neighborhoods to reduce candidates via neighborhood filtering and (ii) an online phase, which further prunes candidates stored in an auxiliary data structure; both phases apply the interlacing theorem on graph Laplacian spectra. Our thorough experimental study shows that, on average, PILOS resolves queries in 19% less time and leaves 23% fewer unresolved queries after a lapse of 10 minutes than the best previous work.
</details>

<details><summary><b>Bio</b></summary>
Konstantinos Skitsas is a PhD student at Aarhus University, where he also obtained his Master’s degree in Computer Science. He obtained a Bachelor's degree from the University of Cyprus. His research focuses on scalable algorithms for graph analysis, including subgraph matching and graph alignment.
</details>

<p>&nbsp;</p>

**Talk 3**: *Nondeterministic Asynchronous Dataflow in Isabelle/HOL*

**Speaker:** Rafael Castro Goncalves Silva

<details><summary><b>Abstract</b></summary>
We formalize nondeterministic asynchronous dataflow networks in Isabelle/HOL. Dataflow networks are comprised of operators that are capable of communicating with the network, performing silent computations, and making nondeterministic choices. We represent operators using a shallow embedding as codatatypes. Using this representation, we define standard asynchronous dataflow primitives, including sequential and parallel composition and a feedback operator. These primitives adhere to a number of laws from the literature, which we prove by coinduction using weak bisimilarity as our equality.
</details>

<details><summary><b>Bio</b></summary>
Rafael Castro G. Silva researches formal verification of software. More precisely, software that manifests "real-world" behavior like side effects, and non-termination. His Ph.D research focuses on verifying stream processing programs, that are usually written using frameworks like Apache Flick and Timely Dataflow. Other topics of his interest are proof assistants, functional programming, and type systems.
</details>

<p>&nbsp;</p>

**Talk 4**: *To be announced*

**Speaker:** Asta Halkjær

<details><summary><b>Abstract</b></summary>
There are many known results in first-order logic: Gödel’s completeness theorem, Gentzen’s Hauptsatz, the compactness theorem, the Löwenheim-Skolem theorem, and Craig’s interpolation theorem. In 1963, Smullyan unified all these results using abstract consistency properties. Later, Fitting adapted them to modal and intuitionistic logics. In this talk, I present abstract abstract consistency properties: a framework developed in Isabelle/HOL for specifying abstract consistency properties for any logic. Using it, we have mechanized completeness of first-order logic with restricted quantifier instantiation, of second-order logic, and of Prior’s Ideal Language, a very strong hybrid logic.
</details>

<details><summary><b>Bio</b></summary>
Asta Halkjær From has a PhD from DTU Compute and is now a postdoc at SDPS. She is sometimes a logician in computer science, and sometimes a computer scientist amongst logicians, but almost always a proof assistant user.
</details>

<p>&nbsp;</p>

### Organisers
- Panagiotis Karras
- Rodrigo Laigner

### Web content
- Rodrigo Laigner
