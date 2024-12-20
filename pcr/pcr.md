{% include head.html %}
![Hanze](../hanze/hanze.png)

[Back to the main page](../index.md)

# Polymerase Chain Reaction

---

![Pic](./pics/impression.jpg)

## Learning outcomes
- Pipetting in μl ranges
- Learning the principle of PCR
- Amplification of DNA with the PCR reaction
- Agarose gel electrophoresis

---
## Preparation
Watch the [following video](https://www.youtube.com/watch?v=iQsu3Kz9NYo) regarding the principle of the PCR reaction.

## Introduction
Polymerase chain reaction (PCR) is a molecular biology method to rapidly amplify a short piece of a specific DNA molecule. The PCR method is a very sensitive method that allows for a very small sample of DNA to be amplified in a large enough amount for analysis by (for instance) electropheresis. Oligonucleotides (or primers) act as starting point for the polymerase reaction. This means that some information about the target sequence is required in order for the PCR reaction to succeed.  

A typical PCR set-up requires several components and reagents:

- a DNA template that contains the DNA target region to amplify
- a DNA polymerase; an enzyme that polymerizes new DNA strands; heat-resistant Taq polymerase is especially common,as it is able to remain intact during the high-temperature DNA denaturation process.
- two DNA primers that are complementary to the 3′ (three prime) ends of each of the sense and anti-sense strands of the DNA target. 
- deoxynucleoside triphosphates, or dNTPs (sometimes called "deoxynucleotide triphosphates"; nucleotides containing triphosphate groups), the building blocks from which the DNA polymerase synthesizes a new DNA strand
- a buffer solution providing a suitable chemical environment for optimum activity and stability of the DNA polymerase together with $Mg^{2+}$-ions. 

The PCR reaction is set up in a small tube and a thermal cycler will facilitate the PCR reaction in the microtube. The PCR reaction consists of several stages (see Figure 1):
- Initialization: This step is only required for DNA polymerases that require heat activation by hot-start PCR (like our VWR Taq polymerase).
- Denaturation: This step is the first regular cycling event and consists of heating the reaction chamber to 95 °C. This causes DNA melting, or denaturation, of the double-stranded DNA template by breaking the hydrogen bonds between complementary bases, yielding two single-stranded DNA molecules.
- Annealing: the reaction temperature is lowered to 50–60 °C allowing annealing of the primers to each of the single-stranded DNA templates. During this stage, the polymerase already extends the primers, albeit at a slower rate, causing the melting temperature of the primers to rise.
- Extension/elongation: The temperature at this step is raised to 72 °C. In this step, the DNA polymerase synthesizes a new DNA strand complementary to the DNA template strand by adding free dNTPs from the reaction mixture that is complementary to the template in the 5′-to-3′ direction.

![Figure 1](./pics/fig1.png)
*<sub>Figure 1: The PCR reaction. Source: Wikipedia.org.</sub>*

After the PCR reaction, a small part of the reaction mixture can be analyzed by agarose electrophoresis. This method is used to separate DNA molecules according to mass. The agarose gel is a three-dimensional matrix formed of agarose molecules aggregated into a three-dimensional structure. This forms a maze of channels and pores through which DNA molecules can pass. DNA migrates towards a positive charge because the molecule is negatively charged due to its abundant phosphate groups. See Figure 2 for loading of an agarose gel.

![Figure 2](./pics/fig2.jpg)
*<sub>Figure 2: Loading of an agarose gel. Source: Wikipedia.org.</sub>*

DNA is visualized by staining with Midori Green, which intercalates into the major grooves of the DNA and fluoresces under UV light. When stained with Midori Green, the gel is viewed with an ultraviolet (UV) transilluminator. The UV light excites the electrons within the aromatic ring of Midori Green, and once they return to the ground state, light is released, making the DNA and Midori Green complex fluoresce (Figure 3).

![Figure 3](./pics/fig3.jpg)
*<sub>Figure 3: Visualization of an agarose gel. Source: Wikipedia.org.</sub>*

## The experiment
We will use the pHIPH4 plasmid to PCR amplify the Hygromycine gene using a forward and reverse primer. 

Primer sequences:  

•	pHIPH4-f: CCCACACACCATAGCTTCAA  
•	pHIPH4-r: CGTTTTCGACACTGGATGGC  

The [sequence of pHIPH4](https://www.addgene.org/117685/) can be found at the addgene website.

## Simulate the PCR
Simulate the PCR using [Benchling](https://www.benchling.com/).
A step-by-step guide can be found [here](https://www.benchling.com/blog/in-silico-pcr-primer-design-and-gene-amplification) and [here](../primer_design/primer_design.md).

Simulate the PCR reaction and record the expected product length in your lab journal.

## Protocol

### Day 1: PCR

Set up a series of PCR reactions. Include a negative control and a positive control according to the table below:

| Sample #| Sample name     |Sample content                        |
|:-------:|:---------------:|:------------------------------------:|
|1        |negative control |PCR-mix + water                       |
|2        |positive control |PCR-mix + pHIPH4 (isolated by teacher)|
|3        |sample           |PCR-mix + pHIPH4 (isolated by student)|

The PCR mix for 50 µL should contain the following:
- 5 µL key buffer
- 1 µl dNTP mix (10 mM each). Create mix from 100 mM stock.
- 10 pmol forward primer. Pipet from 10 μM stock.
- 10 pmol reverse primer. Pipet from 10 μM stock.
- 0.4 µl TEMPase Hot Start DNA Polymerase
- PCR-grade $H_2O$ up to 49 µl.

Then add:
- 1 µl PCR-grade $H_2O$ to tube 1.
- 1 µl PCR product from a 100X-dilluted previous reaction (provided by your supervisor) to tube 2.
- 25 ng of plasmid (pHIPH4) of a 25 ng/µl stock to tube 3. 

PCR conditions:
- Denaturation for 15 minutes at 95˚C (to activate the hot-start polymerase) 
- 30 cycles of:
  - 95˚C for 30 seconds
  - 58˚C for 40 seconds
  - 72˚C for 2 minutes 
- extension step of 5 minutes at 72˚C. 
 

### Day 2: Agarose gel electrophoresis

Proceed with the procedure of [agarose gel electrophoresis](../agarose_gel_electrophoresis/agarose_gel_electropheresis.md)


--- 

>Some  information on this page was adapted and modified from Wikipedia.org.

[Back to the main page](../index.md)

