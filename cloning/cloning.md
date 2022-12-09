{% include head.html %}
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

> Before you start:
We assume that you have basic knowledge and skills about general aseptic techniques in microbiology. It is required that you have obtained a VMT certificate as a start requirement to follow this course!

---

## Introduction
Molecular cloning refers to the process of making multiple ídentical copies of macromolecules such as DNA molecules. Gene cloning is used to amplify DNA fragments containing whole genes. It is used in a wide array of biological experiments such as large scale protein production and vaccin depelopment. 

In many cases, PCR cloning is used to clone a gene. For PCR cloning, primers are designed with 5'-prime extensions that contain restriction sites that match the restriction sites within the multiple cloning site of a particular cloning vector (figure 1). Using two different restriction enzymes with different recognition sequences will facilitate directional cloning of the insert in the vector.

![Figure 1](./pics/fig1.png)
*<sub>Figure 1. Amplification of a gene using PCR. Note that the primers contain a 5'-overhang sequence that matches a restriction site. Source: Addgene.</sub>*

Another (often used) strategy is TA cloning. TA cloning is a cloning technique that avoids the use of restriction enzymes and is easier and quicker than traditional cloning. The technique relies on the ability of adenine (A) and thymine (T) (complementary basepairs) on different DNA fragments to hybridize and, in the presence of ligase, become ligated together. PCR products are usually amplified using Taq DNA polymerase which preferentially adds an adenine to the 3' end of the product. Such PCR amplified inserts are ligated into linearized vectors that have complementary 3' thymine overhangs. An overview of TA cloning can be found in figure 2.

![Figure 2](./pics/fig2.png)
*<sub>Figure 2. Overview of TA cloning. Note that TA cloning eliminates the need of restriction enzymes. Source: Wikipedia.</sub>*


The vector containing the insert is transformed to a cell. Often, a particular strain of *E. coli* (DH5-Alpha) is used for efficient transformation. DH5-Alpha Cells are engineered to maximize transformation efficiency. They are defined by mutations to reduce breakdown of DNA and reduce recombination (endA1, recA1). In addition, the cells facilitate blue white screening. The cells are competent and often used with calcium chloride transformation to insert the desired plasmid. The plasmid contains an "origin of replication" that facilitates replication in the host cell. Transformants (that contain the plasmid DNA) can be selected using an antibiotic selection marker such as the ampicillin resistance gene (figure 3). Transformants with an insert can be selected using blue-white screening. The destination vector contains a part of the β-galactosidase gene (another part of this gene resides in the DH5-Alpha host, the DH5-Alpha strain contains a lacZΔM15 mutation). Ligation of the insert disrupts the β-galactosidase gene on the destination vector. The β-galactosidase part that resides in the DH5-Alpha host does not result in functional β-galactosidase. The presence of active β-galactosidase can be detected by X-gal, a colourless analog of lactose that may be cleaved by β-galactosidase to form a bright blue insoluble pigment. Instead, colonies that contain the insert will remain white as the β-galactosidase gene is disrupted by the precense of the insert. 

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

- x μl 10×PCR reaction buffer
- x μl 10 mM dNTP (dATP, dTTP, dCTP en dGTP; ratio 1:1:1:1)
- x μl 50 mM $MgCl_2$
- x μl 25 pmol/μl primer GFP F
- x μl 25 pmol/μl primer GFP R
- x μl 5 U/μl Taq DNA polymerase
- 10 ng pGLO plasmid DNA en (sterile) MilliQ up to 50 μl

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
- 15 min 95ºC denaturation (this is required to activate VWR TAQ)
- 30 cycles of:
    - 15 seq 95ºC denaturation
    - 45 seq 55ºC annealing
    - 90 seq 72ºC extension
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


### Day 2

#### Agarose gel electrophporesis PCR product
Check 5 μl of the PCR product on a 1% agarose gel. Use an appropriate marker and use loading dye. You can find the procedure for agarose electrophoresis [here](../pcr/pcr.html).
Use your phone to create a picture of the gel on a UV illuminator.

>Be carefull with the UV illuminator. Use a protective mask. 

>If your PCR reaction failed, you can obtain the PCR product from your supervisor. 

#### Cleaning of the PCR product
Clean up the PCR reaction according to the instructions of the kit to remove impurities. Elute in 10 µl elution buffer.

#### Ligation
The optimal ligation ratio for the pGEM®-T vector is 3:1 (insert: vector). use the formula below to calculate the amount of insert needed for 50 ng Vector in your ligation reaction.

$ng\ insert =\frac{ng\ of\ vector\ x\ kb\ size\ of\ insert}{kb\ size\ of\ vector}$

Set up 3 ligation reactions according to table 2:

*<sub>Table 2. Ligation reaction scheme</sub>*

|Reagent                     |gfp-PCR|Pos.Control|background|
|----------------------------|-------|-----------|----------|
|2x rapid DNA Ligation Buffer|5 µl   |5 µl       |5 µl      |
|pGEM®-T (50 ng)             |1 µl   |1 µl       |1 µl      |
|PCR-product                 |x µl   |-          |-         |
|Control DNA                 |-      |1 µl       |-         |
|T4-ligase                   |1 µl   |1 µl       |1 µl      |
|$H2O$ up to 10 µl           |x µl   |x µl       |x µl      |


Mix reactions by pipetting up and down a few times. Place in floaters in a beaker with 1 L of room temperature water. Place in the cold room and incubate overnight.


#### Culture DH5-Alpha Cells
You will receive TY medium that contains:
- 1% (w/v) Bacto-tryptone
- 0.5% (w/v) Bacto yeast extract
- 0.5% NaCl
The medium is autoclaved.

Inoculate 3 mL (use a single colony) of the TY medium with DH5-Alpha cells. Use maximum of 1/5<sup>th</sup> of the culture tube (aeration is very important for growth). Incubate at 37ºC overnight at 220 rpm in a shaker incubator.

### Day 3

#### Preparation competent cells
- Dilute the DH5-Alpha cells 1:100 in 25 mL fresh prewarmed TY medium. Use a sterile Erlenmeyer flask. Use maximum of 1/5<sup>th</sup> of the culture flask in order to make sure that the culture is aerated properly.
- Grow untill OD600 = 0,3 (~1,5- 2 hours)
- Cool 10 min. on ice.
- Centrifuge 10 min at 4°C, 5000 RPM (pre-cool the centrifuge).
- Discard the supernatant. 
- Resuspend the pellet in ice cold 0.1 M $CaCl_2$ (pre-cool this solution) in half of the culture volume. Use a freshly prepared $CaCl_2$ solution (max 1 week old).
- Incubate 30 min. on ice.
- Centrifuge 10 min. at 4°C, 5000 RPM or 30 sec. 12.000 RPM in a tabletop centrifuge (no longer!!). 

>A pellet of competent cells should now be visible. 

- Resuspendend the pellet in ice cold 0.1 M $CaCl_2$ (pre-cool the solution), in 1/100 of the culture volume. 

>Pipet up and down very gently! The cells are susceptible for lysis at this stage.

>Cells are ready for transformation. They will be competent for 30 min. Alternatively, cells can be frozen at -80ºC by adding 87% (v/v) glycerol (17.5 µl 87% (v/v) glycerol for each 100 µl of bacteria suspension).

#### Preparation of plates
Prepare 100 mL medium. You will be able to pour 5 plates.
The recipe for the LB medium:
- 1% (w/v) Bacto-tryptone
- 0.5% (w/v) Bacto-yeast-extract
- 1% NaCl
- 1.5% Agar
Autoclave and cool untill ~ 55°C
Then add:
- 100 µg/mL final concentration Ampicillin (stock is 100 mg/mL)
- 20 µg/mL final concentration X-Gal (stock is 20 mg/mL in DMSO)
- 100 µmol/L final concentration IPTG (stock is 100 mmol/L)

> Why do you need to add? What is the function?
> - Ampicillin
> - X-Gal (hint: search for information about the lac operon)
> - IPTG (hint: search for information about the lac operon)

Pour 5 plates (this means that you will use approximately 20 mL per plate).

#### Transformation
- Mix 25 µl (thawed) competent cells gently by flipping the tube.
- Add 2 µl ligation mixture and mix gently by flipping the tube.
- Incubate for 20 min. on ice.
- Heat-shock the cells for 45-50 seconds at 42°C in a waterbath.
- Incubate for 2 min. on ice.
- Add 900 μl RT LB medium to each transformation-reaction.
- Incubate 60 minutes at 37°C in a shaking incubator at 150 rpm. Position the tubes horizontal. Use tape to fixate the tubes.
- Centrifuge 1 min. at max speed in a Eppendorf centrifuge. Discard most of the supernatant (leave approximately 100 µl) and mix the remaining liquid by pipetting up and down. 
- Use a drigalski spatula to plate the cells on the agar plates.
- Incubate the plates at 37°C overnight.

>Some protocols use SOC medium instead of LB medium. The use of LB medium instead of SOC medium results in a very minor reduction of transformants.

### Day 4

#### Check plate on a UV illuminator
Investigate your plate on a UV illuminator. Use your phone to create a picture of the plate on a UV illuminator.

>Be carefull with the UV illuminator. Use a protective mask.


#### Colony PCR

Choose from the primers depicted in table 3 a primer pair that will detect the insert as well as the orientation of the insert in the vector. Use Benchling to simulate the PCR reactions.

*<sub>Table 3. Available primers</sub>*

|Primer name|Primer sequence (5'&rarr;3')     |
|-----------|---------------------------------|
|M13F       |GTAAAACGACGGCCAGT                |
|M13R       |CAGGAAACAGCTATGACC               |
|GFP F      |GTTTAACTTTAAGAAGGAGATATACATATGG  |
|GFP R      |TTATTTGTAGAGCTCATCCATGCC         |
|Cont. F    |GATGACGGGAACTACAAGAC             |
|Cont. R    |TCGAAAGGGCAGATTGTG               |


Prepare PCR mixtures according to table 4:

*<sub>Table 4. PCR mixtures for colony PCR</sub>*

|Reagent     |[stock]   |[Desired]    |1 reaction (50 µl)|x reactions|
|------------|----------|-------------|------------------|-----------|
|$H_2O$      |-         |-            |up to 50 µl       |           |
|PCR-buffer  |10x       |1x           |                  |           |
|dNTPs       |25 mM     |250 µM       |                  |           |
|Primer F    |25 pmol/µl|25 pmol/50 µl|                  |           |
|Primer R    |25 pmol/µl|25 pmol/50 µl|                  |           |
|MgCl2       |50 mM     |1,5 mM       |                  |           |
|Triton x-100|1%        |0,1%         |                  |           |
|Taq Pol     |5 U/µl    |2-3 U/50 µl  |                  |           |

Divide the master mix in 50 µl aliquots. Keep on ice. Add a tiny bit of a white DH5-Alpha colony material to the tube. Add voth fluorescent and non fluorescent colonies to separate tubes. Do not forget a negative control reaction for each primer pair!

Start the following PCR program:
- 15 min 95ºC denaturation (this is required to activate VWR TAQ)
- 30 cycles of:
    - 15 seq 95ºC denaturation
    - 45 seq 55ºC annealing
    - 90 seq 72ºC extension
- 7 min 72ºC extension
- ∞ at 4ºC

#### Agarose gel elctrophoresis
Check 10 μl of the PCR product on a 1% agarose gel. Use an appropriate marker and use loading dye. You can find the procedure for agarose electrophoresis [here](../pcr/pcr.html).
Use your phone to create a picture of the gel on a UV illuminator.

>Be carefull with the UV illuminator. Use a protective mask.

### At the end
Note the following in your labjournal:
- Number of colonies observed per transformation
- Number and percentage of white and blue colonies (make a table)
- Number and percentage of positive clones for forward and reverse orientation according to the PCR results.
- Number and percentage of fluorescent transformants.
- Number and percentage of white-fluorescent, white non-fluorecent, blue-fluorescent and blue non-fluorescent colonies.

>Dit you find white colonies without green fluorescence?
What could be a reason for this observation?

The end...

--- 

>Some of the text of this webpage is copied, adapted and modified from Wikipedia.org.  
This is an open-access article distributed under the terms of the Creative Commons Attribution License which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited.
Creative Commons License: CC BY-SA 4.0.

---

[Back to the main page](../index.md)

