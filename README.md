# SDPS Summer Conference Rehearsal 2024

On Wednesday, June 12 there will be an event in which everybody interested and willing will practice their chosen forthcoming summer-conference presentation, or any other talk for which feedback and practice is desirable.

### Location:
The event will take place at SCI-DIKU-UP1-01-2-16. 

### Programme:

10:00 - 12:00 **Morning session:** Data Management and Data Streaming 

**[Keynote talk]:** Yijian's PhD

**Title**: *Consistent Data Management Layer on Actor Systems*

<details><summary><b>Abstract</b></summary>
The three-tier architecture is a stalwart in client-server architectures. Its framework divides functionality into presentation,
logic, and data storage layers. Traditionally, the middle tier has hosted application logic, bridging the gap between user interfaces and backend data storage systems. However, a significant shift is underway. More and more applications are embracing a stateful paradigm in the middle tier, where the application state is maintained within the middle tier and asynchronously persisted to the backend storage.

While the practice of keeping data close to the application logic enhances responsiveness and supports high-processing tasks, it also means deviating from the inherent data management capabilities of the database system. These capabilities, such as transaction handling, data replication, and dependency management, are now the responsibility of developers. They are left with the choice of either creating their own data management mechanisms or integrating them directly into the application code. Simultaneously, a trend is emerging of shifting from monolithic structures towards modular, loosely coupled architectures, such as microservices. This architecture brings systems with easier maintenance, independent deployment and scalability, reliability, and diverse technology choices. However, it exacerbates the challenge of managing data across distributed servers.

In light of the critical challenge and urgent need to manage data in the stateful middle tier, this project aims to provide an efficient and scalable data management solution for data-intensive, distributed, and large-scale applications. This project establishes a data management layer on top of the actor system, integrating an expressive data model for actor state management, a novel transaction library and transaction programming abstraction for multi-actor multi-server transactions, an actor migration mechanism for scaling systems while preserving consistent transactional guarantees, and an actor-oriented transactional log replication method.
</details>

<details><summary><b>Bio</b></summary>
Yijian Liu is currently a PhD student in Department of Computer Science at Copenhagen University. She is supervised by professor Yongluan Zhou. Her research work mainly focuses on building efficient and scalable data management solutions on actor systems. One of her research work “Hybrid Deterministic and Nondeterministic Execution of Transactions in Actor systems” was published in a top conference Sigmod in 2022. Her other works are bringing more database features to the stateful actor-oriented application layer.
</details>

**Talk 1:** Rodrigo Laigner

**Title**: *Benchmarking Data Management Systems for Microservices* 

<details><summary><b>Abstract</b></summary>
Microservice architectures emerged as a popular architecture for designing scalable distributed applications. Although microservices have been extensively employed in industry settings for over a decade, there is little understanding of the data management challenges that arise in these applications. As a result, it is difficult to advance data system technologies for supporting microservice applications. 

To fill this gap, we present *Online Marketplace*, a microservice benchmark that incorporates core data management challenges that existing benchmarks have not sufficiently addressed. These challenges include transaction processing, query processing, event processing, constraint enforcement, and data replication. We have defined criteria for various data management issues to enable proper comparison across data systems and platforms.

After specifying the benchmark, we present the challenges we faced in creating workloads that accurately reflect the dynamic and distributed state of the microservices. We also discuss issues that we encountered when implementing *Online Marketplace* in state-of-the-art data platforms and meeting the criteria. Our evaluation demonstrates that the benchmark is a valuable tool for testing important properties sought by microservice practitioners. As a result, our proposed benchmark will facilitate the design of future data systems to meet the expectations of microservice practitioners.
</details>

<details><summary><b>Bio</b></summary>
Rodrigo Laigner is a PhD fellow in the Department of Computer Science at University of Copenhagen under the supervision of Prof. Yongluan Zhou. His research targets building efficient and consistent database systems for data management requirements found in modern data-intensive applications, such as those following the microservice architectural style. 
</details>

**Talk 2:** Rafael Castro Goncalves Silva

**Title**: *Verified Time-Aware Stream Processing*

<details><summary><b>Abstract</b></summary>
Stream processing frameworks provide programming abstractions that allow their users to express the desired time-dependent data analysis. The frameworks organize the computation as a directed graph of interconnected operators that perform event-wise transformations. We tackle the correctness question for programs expressed in this way. To this end, we model (possibly stateful) operators and define their composition, model data streams with time-stamps and watermarks, define reusable, modular operators, and prove their correctness in the Isabelle/HOL proof assistant, taking advantage of its advanced coinductive methods infrastructure. We demonstrate the usefulness of our model by verifying stream processing algorithms computing incremental histograms and relational join.
</details>

<details><summary><b>Bio</b></summary>
Rafael Castro G. Silva researches formal verification of software. More precisely, software that manifests "real-world" behavior like side effects, and non-termination. His Ph.D research focuses on verifying stream processing programs, that are usually written using frameworks like Apache Flick and Timely Dataflow. Other topics of his interest are proof assistants, functional programming, and type systems.
</details>

12:00 - 13:00 **Lunch Break**

13:00 - 14:00 **Afternoon session 1:** Runtime Monitoring and AI

**Talk 3:** Leonardo Lima

**Title**: *WhyMon: A Runtime Monitoring Tool with Explanations as Verdicts*

<details><summary><b>Abstract</b></summary>
I will present WhyMon, a runtime monitoring tool that produces explanations as verdicts. Receiving as input a metric first-order temporal logic (MFOTL) formula and a stream prefix of time-stamped data-carrying events, WhyMon incrementally outputs explanations that describe why each variable assignment satisfies or violates the formula. The tool includes a graphical user interface that facilitates the exploration and understanding of these explanations. Additionally, it incorporates a formally verified checker that can certify the
explanations. I will demonstrate WhyMon's usage throughout the talk.
</details>


<details><summary><b>Bio</b></summary>
I am a PhD student in Computer Science at the University of Copenhagen, under the supervision of Dmitriy Traytel. I am interested in building reliable systems. Hence, I do (research in) formal methods. I started my research endeavours in the areas of proof theory and interactive theorem proving. Nowadays I spend most of my time doing research in runtime verification. I am particularly interested in the development of explainable runtime monitoring tools.
</details>

**Talk 4:** Hubert D. Zając

**Title**: *"It depends": Configuring AI to Improve Clinical Usefulness Across Contexts*


<details><summary><b>Abstract</b></summary>
Artificial Intelligence (AI) repeatedly match or outperform radiologists in lab experiments. However, real-world implementations of radiological AI-based systems are found to provide little to no clinical value. This paper explores how to design AI for clinical usefulness in different contexts. We conducted 19 design sessions and design interventions with 13 radiologists from 7 clinical sites in Denmark and Kenya, based on three iterations of a functional AI-based prototype. Ten sociotechnical dependencies were identified as crucial for the design of AI in radiology. We conceptualised four technical dimensions that must be configured to the intended clinical context of use: AI functionality, AI medical focus, AI decision threshold, and AI Explainability. We present four design recommendations on how to address dependencies pertaining to the medical knowledge, clinic type, user expertise level, patient context, and user situation that condition the configuration of these technical dimensions.
</details>


<details><summary><b>Bio</b></summary>
Hubert D. Zając did his PhD on healthcare AI in Denmark and Kenya. He spent his fair share creating value for shareholders as a UX designer and software developer, which motivated him to try creating value for society instead. He is now a Postdoc at the University of Copenhagen researching methods of realisation of AI in the industry, and a member of the Confronting Data Co-Lab. He is interested in exploring the truth behind medical data, especially how data is collected, designed, labelled, and used. His research and passions also converge in exploring the challenges and opportunities of applying AI in real-world settings. He is always up for a chat about data creation, AI, or the real-world inadequacy of heatmaps.
</details>

14:00 - 14:30 **Coffee Break**

14:30 - 16:00 **Afternoon session 2:** Forthcoming IJCAI talks

**Talk 1:** Petros Petsinis

**Title**: *Seed Selection in the Heterogeneous Moran Process*


<details><summary><b>Abstract</b></summary>
The Moran process is a classic stochastic process that models the rise
and takeover of novel traits in network-structured populations. In
biological terms, a set of mutants, each with fitness m ∈ (0, ∞) invade
a population of residents with fitness 1. Each agent reproduces at a
rate proportional to its fitness and each offspring replaces a random
network neighbor. The process ends when the mutants either fixate (take
over the whole population) or go extinct. The fixation probability
measures the success of the invasion. To account for environmental
heterogeneity, we study a generalization of the Standard process, called
the Heterogeneous Moran process. Here, the fitness of each agent is
determined both by its type (resident/mutant) and the node it occupies.
We study the natural optimization problem of seed selection: given a
budget k, which k agents should initiate the mutant invasion to maximize
the fixation probability? We show that the problem is strongly
inapproximable: it is NP-hard to distinguish between maximum fixation
probability 0 and 1. We then focus on mutant-biased networks, where each
node exhibits at least as large mutant fitness as resident fitness. We
show that the problem remains NP-hard, but the fixation probability
becomes submodular, and thus the optimization problem admits a greedy (1
− 1/e)-approximation. An experimental evaluation of the greedy algorithm
along with various heuristics on real-world data sets corroborates our
results.
</details>


<details><summary><b>Bio</b></summary>
Petros Petsinis is a PhD student at the Computer Science Department of Aarhus University in Denmark. He obtained his bachelor’s degree from the Department of Informatics, AUTH Greece (2020). He also holds a master’s degree in computer science from the Department of Informatics and Telecommunications, NKUA Greece (2022). His main interests are in the area of network analysis, artificial intelligence, and combinatorial optimization.
</details>

**Talk 2:** Xikun Jiang

**Title**: *Privacy-Preserving UCB Decision Process Verification via zk-SNARKs*


<details><summary><b>Abstract</b></summary>
With the increasingly widespread application of machine learning, how to
strike a balance between protecting the privacy of data and algorithm
parameters and ensuring the verifiability of machine learning has always
been a challenge. This study explores the intersection of reinforcement
learning and data privacy, specifically addressing the Multi-Armed
Bandit (MAB) problem with the Upper Confidence Bound (UCB) algorithm. We
introduce zkUCB, an innovative algorithm that employs the Zero-Knowledge
Succinct Non-Interactive Argument of Knowledge (zk-SNARKs) to enhance
UCB. zkUCB is carefully designed to safeguard the confidentiality of
training data and algorithmic parameters, ensuring transparent UCB
decision-making.
Experiments highlight zkUCB’s superior performance, attributing its
enhanced reward to judicious quantization bit usage that reduces
information entropy in the decision-making process. zkUCB’s proof size
and verification time scale linearly with the execution steps of zkUCB.
This showcases zkUCB’s adept balance between data security and
operational efficiency. This approach contributes significantly to the
ongoing discourse on reinforcing data privacy in complex decision-making
processes, offering a promising solution for privacy-sensitive applications.
</details>


<details><summary><b>Bio</b></summary>
Xikun Jiang is a Postdoctoral Fellow at the University of Copenhagen and
part of the Software, Data, People & Society (SDPS) Section. Her
research lies in the intersection of economics, data science, and
machine learning. In particular, she focuses on designing algorithms for
novel techniques in data trading. Additionally, she is also interested
in verifiable machine learning and blockchain.
</details>

**Talk 3:** Petros Petsinis

**Title**: *Robust Reward Placement under Uncertainty*


<details><summary><b>Abstract</b></summary>
We consider a problem of placing generators of rewards to be collected
by randomly moving agents in a network. In many settings, the precise
mobility pattern may be one of several possible, based on parameters
outside our control, such as weather conditions. The placement should be
robust to this uncertainty, to gain a competent total reward across
possible networks. To study such scenarios, we introduce the Robust
Reward Placement problem (RRP). Agents move randomly by a Markovian
Mobility Model with a predetermined set of locations whose connectivity
is chosen adversarially from a known set Π of candidates. We aim to
select a set of reward states within a budget that maximizes the minimum
ratio, among all candidates in Π, of the collected total reward over the
optimal collectable reward under the same candidate. We prove that RRP
is NP-hard and inapproximable, and develop Ψ-Saturate, a
pseudo-polynomial time algorithm that achieves an ϵ-additive
approximation by exceeding the budget constraint by a factor that scales
as O(ln |Π|/ϵ). In addition, we present several heuristics, most
prominently one inspired by a dynamic programming algorithm for the
max–min 0–1 KNAPSACK problem. We corroborate our theoretical analysis
with an experimental evaluation on synthetic and real data.
</details>


<details><summary><b>Bio</b></summary>
Petros Petsinis is a PhD student at the Computer Science Department of
Aarhus University in Denmark. He obtained his bachelor’s degree from the
Department of Informatics, AUTH Greece (2020). He also holds a master’s
degree in computer science from the Department of Informatics and
Telecommunications, NKUA Greece (2022). His main interests are in the
area of network analysis, artificial intelligence, and combinatorial
optimization.
</details>

16:00 **End of Scientific Programme**

### Organisers
- Panagiotis Karras

### Web content
- Rodrigo Laigner
