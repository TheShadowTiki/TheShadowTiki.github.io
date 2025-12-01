# **PAGE 1: HOME (index.html)**

## **\[HERO SECTION\]**

Abdul-Malik Zekri  
Barry Goldwater Scholar | B.S. Computer Engineering & B.A. Mathematics  
Researcher at University of South Florida  
Former Undergraduate Research Fellow, Cold Spring Harbor Laboratory  
\[Download CV\] \[GitHub\] \[LinkedIn\] \[Email\]

## **\[THE RESEARCH HOOK\]**

Research Focus  
I study the algorithmic theory of neural circuits, seeking to bridge the gap between low-dimensional neural manifolds and mechanistic spiking neural network (SNN) substrates. My goal is to understand how circuit topology and dynamics give rise to flexible cognitive functions like decision-making and latent state inference.

## **\[LATEST UPDATES / NEWS\]**

* **March 2025:** Selected as a **Barry Goldwater Scholar**.  
* **June 2025:** Joined **Cold Spring Harbor Laboratory (CSHL)** as an Undergraduate Research Fellow in the Zador Lab.  
* **May 2025:** New preprint on *Walking the Weight Manifold* released on arXiv.

# **PAGE 2: RESEARCH (research.html)**

## **\[OVERVIEW\]**

**The Question:** How do biological circuits implement the computation required for flexible behavior?

My work combines mathematical theory, high-performance computing, and biological constraints to investigate the mechanistic basis of neural computation. I am specifically interested in how neural circuits infer and maintain latent representations of the environment to support zero-shot and few-shot learning.

## **\[CORE THEMES\]**

### **1\. Neural Manifolds & Mechanistic Substrates**

While the field often studies neural manifolds in abstract rate-based models, I aim to anchor these concepts in biological constraints.

* **Goal:** Develop a bridge between low-dimensional population dynamics and specific connectivity motifs in Spiking Neural Networks (SNNs).  
* **Approach:** Using "in silico" models as testbeds to unify control theory, dynamical systems, and STDP-based learning rules.

### **2\. Latent State Inference & Cognitive Flexibility**

Animals can adapt to novel scenarios with minimal experience, suggesting they use "latent states" to represent context.

* **Hypothesis:** Circuits do not just overwrite synaptic weights during learning; they shift and modulate existing manifolds to represent new task rules.  
* **Application:** Studying **Reversal Learning** and **Flexible Decision-Making** to understand how networks balance stability (remembering old tasks) with plasticity (learning new ones) without catastrophic interference.

## **\[TOOLBOX\]**

* **Theory:** Dynamical Systems, Graph Theory, Information Geometry.  
* **Computation:** JAX/Flax for differentiable physics; CUDA for parallel acceleration.  
* **Modeling:** Leaky Integrate-and-Fire (LIF) networks, Recurrent Neural Networks (RNNs), Evolutionary Optimization.

# **PAGE 3: PUBLICATIONS (publications.html)**

*Authorship Key: **A.M. Zekri** denotes equal contribution or primary authorship where applicable.*

## **\[PREPRINTS\]**

Walking the Weight Manifold: A Topological Approach to Conditioning Inspired by Neuromodulation  
A. Benjamin, K. Daruwalla, C. Pehle, A.-M. Zekri, and A. M. Zador.  
arXiv preprint arXiv:2505.14635 (2025).  
\[PDF\] \[Code\] \[Abstract\]  
Bridging Predictive Coding and MDL: A Two-Part Code Framework for Deep Learning  
B. Prada, S. Matsumoto, A.-M. Zekri, and A. Mali.  
arXiv preprint arXiv:2505.22994 (2025).  
\[PDF\] \[Code\]

## **\[MANUSCRIPTS IN PREPARATION\]**

Semi-Automated Human-in-the-Loop Proofreading Workflow for the Instance Segmentation of Mitochondria  
A.-M. Zekri, E. Amick, G. Spirou, T. J. Fawcett.  
Manuscript in preparation.

## **\[SELECTED CONFERENCE PRESENTATIONS\]**

### **Oral Presentations**

Neuromodulation-Inspired Conditioning for Reinforcement Learning Tasks  
A.-M. Zekri, A. Benjamin, A. M. Zador.  
Gulf Coast Undergraduate Research Symposium (GCURS), Houston, TX, 2025\.

### **Poster Presentations**

Evolutionary Optimization of Biologically Inspired Mechanistic Input-Output Neural Circuit Models  
A.-M. Zekri, A. Mali.  
National Conference on Undergraduate Research (NCUR), Pittsburgh, PA, 2025\.  
Automated Proofreading Workflow for Mitochondria Segmentation in EM Volumes  
A.-M. Zekri, E. Amick, G. Spirou, T. J. Fawcett.  
10th Annual BRAIN Initiative Conference, Rockville, MD, 2024\.

# **PAGE 4: PROJECTS (projects.html)**

## **\[FEATURED RESEARCH PROJECTS\]**

### **Neuromodulation on Weight Manifolds**

*CSHL (Zador Lab) | Python, JAX, Flax, Brax, PPO*

* **Problem:** Standard Reinforcement Learning (RL) struggles to generalize to related tasks without extensive retraining.  
* **Method:** Implemented a generalized model of neuromodulation that navigates a "weight manifold" rather than optimizing single weights. Engineered custom wrappers in **JAX/Brax** to integrate this manifold approach with Proximal Policy Optimization (PPO).  
* **Outcome:** Created transformation-safe architectures for continuous control tasks and visualized the optimization landscape using Manim. (See Preprint).

### **Evolutionary Optimization of SNNs**

*TKAI Lab (Mali Lab) | Python, Brian2, Evolutionary Algorithms*

* **Problem:** Linking mechanistic spiking activity to functional input-output behavior in the auditory pathway.  
* **Method:** Utilized **CNModel** to generate synthetic cochlear nucleus spike trains. Applied evolutionary meta-heuristic algorithms to optimize parameters of biologically plausible Spiking Neural Networks (SNNs) with STDP learning rules.  
* **Outcome:** Demonstrated convergence of mechanistic models toward biological reference data; presented at NCUR 2025\.

### **High-Performance Connectomics Pipeline**

*ADCL (Spirou Lab) | Python, SLURM, Deep Learning (CDeep3M)*

* **Problem:** Segmenting mitochondria in Electron Microscopy (EM) volumes is a bottleneck for 3D reconstruction.  
* **Method:** Developed a semi-automated "Human-in-the-Loop" proofreading workflow. Implemented HPC workflows using **SLURM** to parallelize deep learning segmentation across large image volumes.  
* **Outcome:** Significantly improved segmentation accuracy and efficiency; presented at the BRAIN Initiative Conference.

### **GPU-Accelerated Graph Search (HNSW)**

*HPC Lab (Tu Lab) | C++, CUDA, Parallel Computing*

* **Problem:** Nearest neighbor search in large-scale biological databases (e.g., DNA alignment) is computationally expensive.  
* **Method:** Designed a parallelized search algorithm for Hierarchical Navigable Small World (HNSW) graphs. Optimized memory access patterns and thread divergence on NVIDIA GPUs.  
* **Outcome:** Achieved significant speedup over CPU-only implementations.

# **PAGE 5: ABOUT (about.html)**

## **\[MOTIVATION: THE SYSTEMS LENS\]**

I came to neuroscience via mathematics and logic, driven by a fascination with how rigorous formal systems give rise to the messiness of adaptive behavior.

My intellectual inflection point occurred during a course on **Computer Architecture**, where we systematically analyzed the datapath and control logic powering the fetch-decode-execute cycle. Understanding how a computer’s complex function emerges from structured components with defined roles reshaped how I view the brain.

Since we cannot yet build a brain in the lab, I chose the next best path: acquiring the mathematical and computational tools to model its principles *in silico*. I view the brain through a "systems lens"—where solutions to complex problems (like water scarcity or motor control) are found not in the components themselves, but in their topological organization and dynamic interplay.

## **\[INTEGRATED RESEARCH APPROACH\]**

My objective is to investigate neural computation by integrating **structure**, **dynamics**, and **theory**. My undergraduate research has focused on building competence in each of these distinct levels of analysis:

1\. The Structural Hardware (Connectomics)  
At the ADCL (Spirou Lab)  
To understand the circuit, we must first map the wires. My work in EM segmentation and High-Performance Computing has focused on characterizing the structural constraints that limit and guide neural computation.  
2\. The Dynamical Software (Manifolds & SNNs)  
At CSHL (Zador Lab) & TKAI (Mali Lab)  
Structure enables dynamics. At CSHL, I investigated how weight manifolds support generalization, and at TKAI, I am using evolutionary algorithms to identify the specific biological motifs that allow stable population dynamics to emerge from static connectivity.  
3\. The Theoretical Objective (MDL & Predictive Coding)  
At TKAI (Mali Lab)  
Dynamics must serve a purpose. I am exploring theoretical frameworks like Minimum Description Length (MDL) and Predictive Coding to explore the normative principles guiding learning—investigating how circuits might optimize information efficiency to build latent representations of the world.

## **\[FUTURE OUTLOOK\]**

As a PhD student, I aim to advance mechanistic models of cognition. By investigating the circuit-level principles of latent state inference, I hope to contribute to the design of interpretable, energy-efficient AI and explore principled rewiring strategies for restoring function in neurological disorders.

# **PAGE 6: LEADERSHIP & OUTREACH (leadership.html)**

## **\[PHILOSOPHY\]**

Scientific progress requires sustainable intellectual infrastructure. My approach to leadership is systems-based: identifying bottlenecks in the research ecosystem—whether in knowledge access, student training, or interdisciplinary collaboration—and designing structural solutions to address them.

## **\[KNOWLEDGE TRANSLATION & COMMUNICATION\]**

PaperADay (In Development)  
Founder & Lead  
A forthcoming science communication initiative designed to lower the activation energy required to engage with primary literature.

* **Vision:** "Make real science (science literature) fun and exciting for everyone, every day."  
* **Mechanism:** Developing a platform to translate dense computational neuroscience papers into accessible, daily summaries that retain technical rigor while stripping away jargon barriers.

Research Chalk Talks & Journal Clubs  
Discussion Lead  
I prioritize the skill of "board-work" communication—explaining complex mathematical concepts (e.g., linear algebra, dynamical systems) in real-time without slides. I regularly organize and lead peer discussions to practice translating formal proofs into intuitive physical arguments.

## **\[RESEARCH CULTURE & INSTITUTION BUILDING\]**

STEMCORE (STEM Collaboration and Research Initiative)  
Founder & President  
Identified a structural gap in undergraduate research access: motivated students often lack the specific technical skills required to join computational labs.

* **Action:** Founded an interdisciplinary organization to provide "on-ramp" training.  
* **Impact:** Organized technical seminar series and skill-building workshops, creating a pipeline for students to acquire research-ready skills before applying to labs.

Bioinformatics Club  
President  
Lead the organization of technical workshops and guest lectures, fostering a community of practice for students at the intersection of biology and computer science.

## **\[ACADEMIC MENTORSHIP\]**

Honors College Peer Mentor & Learning Assistant  
University of South Florida  
Formal instruction and mentorship roles for the Honors Foundations and Cancer Biology courses.

* **Role:** Facilitated discussion sections and guided first-year honors students in developing academic strategies.  
* **Objective:** To move beyond content delivery and teach the *metacognitive* skills required for rigorous academic inquiry.

PAMSA Tutoring Officer  
Designed and managed tutoring structures to support student success in pre-medical and science coursework.

## **\[CIVIC SYSTEMS DESIGN\]**

Mayor's Youth Leadership Council  
Tampa, FL  
Early experience in civic systems design. Worked with city officials to analyze community needs and design structural interventions for youth engagement. This experience grounded my belief that effective leadership requires understanding the system before attempting to optimize it.