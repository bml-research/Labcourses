![Hanze](../hanze/hanze.png)

[Back to the main page](../index.md)

# Cloning

---

![Pic](./pics/impression.png)

## Learning outcomes
- Pipetting in μl ranges
- Cutting DNA with restriction enzymes
- Ligation of DNA
- Creating competent *E. coli*
- Transformation of bacteria
- Selection of recombinant clones

---

>Some of the text of this webpage is copied, adapted and modified from Wikipedia.org.  
This is an open-access article distributed under the terms of the Creative Commons Attribution License which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited.
Creative Commons License: CC BY-SA 4.0.

---

## Introduction
Molecular cloning refers to the process of making multiple ídentical copies of macromolecules such as DNA molecules. Gene cloning is used to amplify DNA fragments containing whole genes. It is used in a wide array of biological experiments such as large scale protein production and vaccin depelopment. 

In many cases, PCR cloning is used to clone a gene. For PCR cloning, primers are designed with 5'-prime extensions that contain restriction sites that match the restriction sites within the multiple cloning site of a particular cloning vector (figure 1). Using two different restriction enzymes with different recognition sequences will facilitate directional cloning of the insert in the vector.

![Figure 1](./pics/fig1.png)
*<sub>Figure 1. Amplification of a gene using PCR. Note that the primers contain a 5'-overhang sequence that matches a restriction site. Source: Addgene.</sub>*

Another (often used) strategy is TA cloning. TA cloning is a cloning technique that avoids the use of restriction enzymes and is easier and quicker than traditional cloning. The technique relies on the ability of adenine (A) and thymine (T) (complementary basepairs) on different DNA fragments to hybridize and, in the presence of ligase, become ligated together. PCR products are usually amplified using Taq DNA polymerase which preferentially adds an adenine to the 3' end of the product. Such PCR amplified inserts are ligated into linearized vectors that have complementary 3' thymine overhangs. An overview of TA cloning can be found in figure 2.

![Figure 2](./pics/fig2.png)
*<sub>Figure 2. Overview of TA cloning. Note that TA cloning eliminates the need of restriction enzymes. Source: Wikipedia.</sub>*


The vector containing the insert is transformed to a cell. Often, a particular strain of *E. coli* (DH5-Alpha) is used for efficient transformation. DH5-Alpha Cells are engineered to maximize transformation efficiency. They are defined by mutations to reduce breakdown of DNA and reduce recombination. In addition, the cells facilitate blue white screening. The cells are competent and often used with calcium chloride transformation to insert the desired plasmid. The plasmid contains an "origin of replication" that facilitates replication in the host cell. Transformants (that contain the plasmid DNA) can be selected using an antibiotic selection marker such as the ampicillin resistance gene (figure 3). Transformants with an insert can be selected using blue-white screening. The destination vector contains a part of the β-galactosidase gene (another part of this gene resides in the DH5-Alpha host). Ligation of the insert disrupts the β-galactosidase gene on the destination vector. The β-galactosidase part that resides in the DH5-Alpha host does not result in functional β-galactosidase. The presence of active β-galactosidase can be detected by X-gal, a colourless analog of lactose that may be cleaved by β-galactosidase to form a bright blue insoluble pigment. Instead, colonies that contain the insert will remain white as the β-galactosidase gene is disrupted by the precense of the insert. 

 At the end of the cloning procedure, the desired DNA can be amplified to large amounts for downstream applications such as recombinant protein production.

![Figure 3](./pics/fig3.png)
*<sub>Figure 3. Transformation and selection of the recombinant vector. Source: Addgene.</sub>*

During this practical course, you will clone the eGFP gene that encodes the green fluorescent protein. The resulting transformants will be fluorescent under an UV light.

The procedure of cloning can be divided in the following steps:
1.	PCR of the DNA fragment (in this particular case, the GFP gene)
2.	Ligation of the PCR product (GFP-gene) in the desired plasmid (pGEM®-T Vector)
3.	Transformation of the vector with insert (pGEM®-T Vector + GFP-gene) in *E. coli* cells
4.	Screening and selection of *E. coli* cells which are tranformed with the plasmid DNA.

## Procedure

### Preparation
Simulate the PCR and cloning procedure in [Benchling](https://www.benchling.com/). Your teacher can provide you with Bio-informatics tutorials regarding the simulation of PCR reactions and cloning in Benchling.


### Day 1

#### PCR

- You will be offered the pGLO plasmid that contains the GFP gene.
- Setup a PCR reaction to amplify the GFP gene. Primers used are:
    - GFP F	5’-GTTTAACTTTAAGAAGGAGATATACATATGG–3’
    - GFP R	5’-TTATTTGTAGAGCTCATCCATGCC–3’

>Identify the two restriction sites in the primers.

The sequence of the pGLO vector can be found here:
https://www.addgene.org/vector-database/6569/

>Download the sequence in GeneBank format. Use benchling to simulate the PCR. What is the size of the amplicon (PCR product)?

The recipe for the PCR reaction (50 µl):

•	x μl 10×PCR reaction buffer, 
•	x μl 10 mM dNTP (dATP, dTTP, dCTP en dGTP; ratio 1:1:1:1),
•	x μl 50 mM $MgCl_2$,
•	x μl 25 pmol/μl primer GFP F,
•	x μl 25 pmol/μl primer GFP R,
•	x μl 5 U/μl Taq DNA polymerase,
•	10 ng pGLO plasmid DNA en (sterile) MilliQ up to 50 μl.

>Assignment
•	Fill in the missing fields of table 1. 
•	In order to end with enough PCR procuct, 3 reactions will be used. In addition, a negative control reaction will be used. What will you use as a negative control? 

*<sub>Table 1. PCR reaction scheme</sub>*

|Reagentia |stock concentration|desired concentration|Volume for 50 µl reaction|number of reactions|
|----------|-------------------|---------------------|-------------------------|-------------------|
|$H_2O$       |NA                 |NA                   |                         |                   |
|Taq-buffer|10x                |1x                   |                         |                   |
|dNTPs     |25 mM              |250 µM               |                         |                   |
|GFP-F primer|25 pmol/µl       |25 pmol/50µl         |                         |                   |
|GFP-R primer|25 pmol/µl       |25 pmol/50µl         |                         |                   |
|$MgCl_2$  |50 mM              |1.5 mM               |                         |                   |
|Taq Pol   |5 U/µl             |2 U/50 µl            |                         |                   |
|Template  |25 ng/µl           |100 ng/50µl          |                         |                   |


The PCR program is as follows:
- 1 min 95ºC denaturation
- 30 cycles of:
    - 1 min 95ºC denaturation
    - 1 min 55ºC annealing
    - 1 min 72ºC extension
- 7 min 72ºC extension
- ∞ at 4ºC

Prepare on ice.
Make use of the hot start option.
Transfer the tubes once the heating block reaches 95ºC.


#### Plasmid isolation
You will receive an overnight culture of *E. coli* that contains the destination plasmid (pGEM<sup>®</sup>-T vector).

The vector sequence can be found here: https://www.addgene.org/vector-database/2854/

Use 2 mL of the culture for plasmid isolation.
The procedure for plasmid isolation can be found [here](../nucleic_acid_isolation/nucleic_acid_isolation.html).

Measure the concentration of the plasmid DNA on the nanodrop.

#### Culture DH5-Alpha Cells
You will receive TY medium that contains:
- 1% (w/v) Bacto-tryptone
- 0.5% (w/v) Bacto yeast extract
- 0.5% NaCl
The medium is autoclaved.

Inoculate 3 mL (use a single colony) of the TY medium with DH5-Alpha cells. Use maximum of 1/5<sup>th</sup> of the culture tube (aeration is very important for growth). Incubate at 37ºC overnight at 220 rpm in a shaker incubator.


### Day 2

#### Culture competent cells
Dilute the DH5-Alpha cells 1:100 in 25 mL fresh prewarmed TY medium. Use a sterile Erlenmeyer flask. Use maximum of 1/5<sup>th</sup> of the culture flask in order to make sure that the culture is aerated properly.

#### Agarose gel electrophporesis PCR product
Check 5 μl of the PCR product on a 1% agarose gel.
You can find the procedure for agarose electrophoresis [here](../pcr/pcr.html). If your PCR reaction failed, you can obtain the PCR product from your supervisor. Incubate at 37ºC at 220 rpm in a shaker incubator for 3 hours.

#### Cleaning of the PCR product
Clean up the PCR reaction according to the instructions of the kit to remove impurities. Elute in 10 µl elution buffer.

#### Ligation
The optimal ligation ratio for the pGEM®-T vector is 3:1 (insert: vector). use the formula below to calculate the amount of insert needed for 50 ng Vector in your ligation reaction.

$ng\ insert =\frac{ng\ of\ vector\ x\ kb\ size\ of\ insert}{kb\ size\ of\ vector}$

Set up 3 ligation reactions according to table 2:

*<sub>Table 2. Ligation reaction scheme</sub>*




--- 

[Back to the main page](../index.md)

<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    tex2jax: {
      inlineMath: [ ['$','$'], ["\\(","\\)"] ],
      processEscapes: true
    }
  });
</script>
    
<script type="text/javascript"
        src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>