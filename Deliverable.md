# **Assignment: Designing a Genetic Circuit for live biotherapeutics organism *Escherichia coli Nissle 1917 (EcN)* **

## **Background**
Engineered probiotics are emerging as “live biotherapeutics”. Because of complex interactions in microbial communities, a harmless microbe can become a pathogen in the presence of a specific microbial species or when environmental conditions change. In such cases, it is desirable to have a therapeutic that is only activated under very specific conditions. One possible solution is to engineer a microbe that produces an antimicrobial agent (e.g., an anti-biofilm enzyme, a bacteriocin, or a CRISPR-based kill switch) only when a defined combination of signals is present.

In recent years, synthetic biology tools have made it possible to turn harmless Escherichia coli Nissle 1917 (EcN) into a “living drug.” The idea is to equip the bacterium with a genetic circuit, similar to an electronic circuit. This circuit consists of DNA parts that can sense signals, process them using logical rules (such as AND, OR, NOT), and activate a therapeutic gene only when the correct conditions are met.

Many bacteria communicate with each other through a process called quorum sensing. In this process, each cell releases small signaling molecules into its environment. As the number of cells increases, the concentration of these molecules rises. Once a certain threshold concentration is reached, the molecules bind to specific proteins inside the cells, which then regulate gene expression. In this way, bacteria can coordinate their behavior depending on how many cells are present.

Two intestinal microorganisms of interest that can become pathogenic are *Pseudomonas aeruginosa* and *Yersinia enterocolitica*. Both use quorum sensing systems based on N-acyl homoserine lactones (AHLs).
*Pseudomonas aeruginosa* produces the signaling molecule C12 (3OxoC12-AHL), which binds to the transcriptional regulator LasR. Once activated, LasR induces expression of the enzyme LasI. LasI then produces more C12, creating a positive feedback loop that strengthens the signal as the population grows.
In contrast, *Yersinia enterocolitica* produces a different AHL molecule (C6-AHL), which is sensed by the regulatory protein EsaR. This protein represses gene expression in the absence of C6, and this repression is relieved when C6 is present.

![image1](Figures/deliverable_system.png)
 **Figure 1** Transcriptional regulation of LasR and EsaR. Figure obtained from Li et al. (2025)

## **Objective**
Your task is to design a genetic circuit that enables EcN to respond produce anti-microbial agents when both C12 and C6 are present.
You only have to design the genetic circuit, the gene producing the antimicrobial agent is given (DspB, bactericidal peptide).
Your submission will include both a design proposal and a biological rationale.

## **Deliverables**
You must submit the following:

1. **Genetic Circuit Design (Core Requirement)**  
   - Define the truth table and Boolean logic required for pathway regulation.
   - Sketch a genetic interaction diagram, showing key components (e.g., promoters, regulators, repressors, activators) and their relationships.
   - Explain your choices for the promoter and regulator, justifying how they lead to production of the antimicrobial.

2. **Biological Rationale (Choose ONE of the following):**
   - **Option A: Potential Challenges and Solutions**  
     - Identify at least one key challenge in implementing your genetic circuit (e.g., metabolic burden, leaky expression, unintended cross-regulation).  
     - Propose a possible solution to mitigate this challenge.  
  
   - **Option B: Application of the Circuit**  
     - Describe how your circuit would behave in a real‑world setting (e.g., a mouse gut, a fermenter, a food‑preservation model)
     - Discuss at least two environmental variables (pH, oxygen, substrate availability) and how your design copes with them.

## **Grading Rubric (Total: 10 points)**

| **Category**                 | **Criteria**                                                  | **Points** |
|------------------------------|---------------------------------------------------------------|------------|
| **Genetic Circuit Design**   | Clear and correct truth table and Boolean logic               | 1          |
|                              | Logical and minimalistic genetic interaction design           | 1          |
|                              | Justification of promoter and regulator choice                | 1          |
| **Biological Rationale**     | Clear and well-supported discussion of selected option        | 3          |
|      | Plausibility of proposed problem and solution                 | 2          |
| **Clarity and Organization** | Well-structured, concise, and free of major errors            | 1          |
|                              | Clear caption and labels of figures and diagrams              | 1          |


**Total: 10 points**

## **Submission Guidelines**
- Submit a single PDF containing your circuit diagram, logic explanation, and biological rationale.
- Name your PDF: `lastname_firstname.pdf`
- Keep your responses concise (max 1 pages, excluding diagrams).
- Label all components in your figures and tables clearly and provide clear and instructive captions.
- Submit your work in Moodle before the 13th of May 2026

By completing this assignment, you will develop a deeper understanding of logic-based gene regulation and its applications in metabolic engineering. Good luck!

