![Hanze](../hanze/hanze.png)

[Back to the main page](../index.md)

# Induction of heat shock mRNA in **Caenorhabditis elegans** by heat shock

---

![Pic](./pics/impression.jpg)

## Learning outcomes
- Isolation of total RNA uising Trizol.
- Synthesis of cDNA.
- Performing qPCR analysis.

---

## Introduction

### **Caenorhabditis elegans** biology and life cycle
**Caenorhabditis elegans** is a well-studied, non-parasitic transparent nematode. *C. elegans* is often mischaracterized as a soil nematode but can most easily be isolated from rotting vegetable matter, which contains an ample supply of their bacterial food source. *C. elegans* can be easily grown in the laboratory using *E. coli* strain OP50 as a food source. 

Newly hatched larvae are 0.25 millimeters long and adults are 1 millimeter long. Their small size means that the animals are usually observed with dissecting microscopes up to 100X magnification. See figure 1 for an overview of *C. elegans* morphology.

*C. elegans* has a rapid life cycle (3 days at 25° from egg to egg-laying adult) and exists primarily as a self-fertilizing hermaphrodite, although males arise at a frequency of <0.2%. These features have helped to make *C. elegans* a powerful model of choice for eukaryotic genetic studies. In addition, because the animal has an precisely defined number of somatic cells, researchers have been able to track the fate of every cell between fertilization and adulthood in live animals and to generate a complete cell lineage. The male *C. elegans*, for example, has 1031 cells, a number which does not change after the end of the larval period. 

As mentioned above, wild-type *C. elegans* has two sexual forms: self-fertilizing hermaphrodites and males. The gonad of hermaphrodites forms an ovotestis that first produces haploid amoeboid sperm that are stored in the spermathecal.  Subsequently, the germ line switches fate to produce oocytes. Essentially hermaphrodites are females whose gonads temporarily produce sperm before they produce oocytes. Hermaphrodites can produce up to 300 self-progeny that are fertilized by the stored sperm. If mated with males, hermaphrodites are capable of producing ~1000 offspring, indicating that hermaphrodite-produced sperm is a limiting factor in self-fertilization. Both sexes are diploid for the five autosomal chromosomes. The sexes differ in that hermaphrodites have two X chromosomes and males have a single X chromosome — *C. elegans* has no Y chromosome — and the genotype of males is referred to as XO. Sex is determined by the X to autosome (X:A) ratio. The majority of offspring produced by self-fertilization are hermaphrodites; only 0.1-0.2% of the progeny are males due to rare meiotic non-disjunction of the X chromosome. 


![Figure 1](./pics/fig1.jpg)
*<sub>Figure 1. Observing *C. elegans*. (A) Petri dishes sitting on the base of a dissecting stereomicroscope. Bacterial lawns are visible on the surface of the agar inside the dishes but the *C. elegans* are too small to be seen in this view. (B) *C. elegans* viewed through the dissecting microscope. The two adults are moving in this view. Tracks in the plate indicate where animals have traveled on the bacterial lawn. (C) An adult hermaphrodite is viewed in a compound microscope. In all pictures, anterior is to the left and ventral is on the bottom. *C. elegans* moves on either its left or right side; in this image the surface facing the viewer is the left side. Because the animals are transparent, one can see, from left to right on the ventral side, developing oocytes in the gonad (rectangular cells with a clear, circular nucleus inside) followed by the spermatheca (where oocytes are fertilized), and multiple embryos in the uterus. (D) Fluorescent image showing the nervous system labeled with a GFP reporter (sto-6::gfp). Photo credits: (C) Original (modified here): B. Goldstein; (D) J. Kratz. Source: http://www.wormbook.org/chapters/www_celegansintro/celegansintro.html</sub>*


Under environmental conditions which are favourable for reproduction, hatched larvae develop through four stages, designated as L1 to L4. *C. elegans* embryogenesis takes approximately 16 hours at 20°C. A virtually impermeable eggshell is made after fertilization, allowing the embryo to develop completely independent of the mother. However, embryos are usually retained within the hermaphrodite until the 24-cell stage at which time they are laid. The hermaphrodite embryo hatches and becomes a first stage (L1) larva. The animals begin to eat and develop through four larval stages (L1-L4). The L1 stage is ~16 hr long; the other stages are ~12 hr long. Each stage ends with a sleep-like period of inactivity called lethargus in which a new cuticle (outer collagenous layer) is made. Lethargus ends with the molting of the old cuticle. Approximately 12 hr after the L4 stage, adult hermaphrodites begin producing progeny for a period of 2-3 days until they have utilized all of their self-produced sperm; additional progeny can be generated if the sperm-depleted hermaphrodite mates with a male. After the reproductive period, hermaphrodites can live several more weeks before dying due to senescence. See figure 2 for an overview of *C. elegans* life cycle.

![Figure 2](./pics/fig2.jpg)
*<sub>Figure 2. Life Cycle of *C. elegans*. Animals increase in size throughout the four larval stages, but individual sexes are not easily distinguished until the L4 stage. At the L4 stage, hermaphrodites have a tapered tail and the developing vulva (white arrowhead) can be seen as a clear half circle in the center of the ventral side. The males have a wider tail (black arrowhead) but no discernable fan at this stage. In adults, the two sexes can be distinguished by the wider girth and tapered tail of the hermaphrodite and slimmer girth and fan-shaped tail (black arrowhead) of the male. Oocytes can be fertilized by sperm from the hermaphrodite or sperm obtained from males through mating. The dauer larvae are skinnier than all of the other larval stages. Photographs were taken on Petri dishes (note the bacterial lawns in all but the dauer images). Bar 0.1 mm. Source: http://www.wormatlas.org/ver1/handbook/anatomyintro/anatomyintro.htm</sub>*

When bacteria are depleted and the animals are crowded, L2 larvae activate an alternative life cycle and moult into an alternative L3 larval stage called the “dauer” larva (“dauer” in German means “lasting"). The dauer larva show enhanced resistance to starvation conditions and chemicals. Dauer larvae can survive for many months and are the dispersal form most commonly encountered in the wild. When the dauer larvae are transferred onto plates with bacteria, they continue their development. 

### *Caenorhabditis elegans* anatomy

Figure 3 shows a cartoon of the anatomy of *C. elegans*. *C. elegans* lacks a respiratory and a circulatory system. However, the animal contains an epidermis, muscles and a digestive tract. The outer epithelial layer, the epidermis, of the embryo undergoes a series of cell fusions to make large multinucleate, or syncytial, epidermal cells. These cells secrete the cuticle, a protective layer of specialized extracellular matrix (ECM). The cuticle determines the shape of the body and, through connection from the epidermis to muscle, provides anchoring points for muscle contraction. Just interior and connected to the epidermis are four quadrants of body-wall muscles that run along the length of the body. The regular contraction and relaxation of the muscle cells leads to the “elegant” sinusoidal movement of the animal. In addition to the body-wall muscle, *C. elegans* has muscles that control eating (pharyngeal muscles), egg-laying (vulval and uterine muscles and the contractile gonad sheath), mating (male-specific tail muscles), and defecation (enteric muscles). Food (bacteria) enters the anterior of the animals and passes through the pharynx, a two-lobed neuromuscular pump that grinds the food before it is passed on to the intestine for digestion. The *C. elegans* intestine is attached to the posterior pharynx and consists of 20 large, polyploid epithelial cells arranged in pairs that form a tube running the length of the animal. The nervous system of the adult hermaphrodite has 302 neurons and that of the adult male has 383 neurons. *C. elegans* neurons make more than 7000 chemical synapses and gap junction connections. Although small, the nervous system of *C. elegans* is still relatively complex.

![Figure 3](./pics/fig3.jpg)
*<sub>Figure 3. *C. elegans* anatomy. Major anatomical features of a hermaphrodite (A) and male (B) viewed laterally. (A) The dorsal nerve cord (DNC) and ventral nerve cord (VNC) run along the entire length of the animal from the nerve ring. Two of the four quadrants of body wall muscles are shown. (B) The nervous system and muscles are omitted in this view, more clearly revealing the pharynx and intestine. (C) Cross-section through the anterior region of the *C. elegans* hermaphrodite (location marked with a black line in A) showing the four muscle quadrants surrounded by the epidermis and cuticle with the intestine and gonad housed within the pseudocoelomic cavity. Images modified from those found at www.wormatlas.org</sub>*

## *Caenorhabditis elegans* and the heat shock response

Cells and organisms respond to elevated temperatures by synthesizing a group of highly conserved proteins, the heat shock proteins or HSPs. This response is called the heat shock response. *C. elegans* normally grows at 15-25˚C. Switching the culture to 37˚C for 30 minutes will induce the heat shock response by initializing the transcription of a many heat shock proteins. Directly after the induction of the heat shock response, *C. elegans* is temporary more resistant to heat as a result of elevated heat shock proteins.

The group of heat shock proteins consists, among other proteins, of many different chaperone proteins. Chaperone proteins assist in the folding and assembly of denatured proteins. There are different types of heat shock proteins. Hsp70 belongs to the large heat shock proteins and is a 70 kilo Dalton protein that assists in the refolding of unfolded proteins. In addition to the group of larger heat shock proteins, smaller heat shock proteins exist such as the Hsp16.1 protein. In contrast to the larger heat shock proteins that assist in refolding, the smaller heat shock proteins are generally believed to protect proteins from denaturation by keeping them in a folding competent state and handing them over to the larger chaperones for refolding.

### Real-time PCR

In order to investigate if the transcription of the HSP is upregulated by heat-shock, a real-time PCR analysis will be performed. The procedure can be subdivided in three parts:
1.	RNA isolation
2.	Reverse transcription
3.	Real-time PCR
To investigate the induction of transcription, RNA needs to be isolated. We will isolate the total RNA as this procedure is less complicated compared to the isolation of mRNA. The PCR procedure cannot be performed on RNA. Therefore, the RNA will first be reverse-transcribed to cDNA using reverse-transcriptase. Oligo-dT primers will be used as starting point to initiate the cDNA reaction. Oligo-dT primers will bind the poly(A) tail. As both rRNA and tRNA do not contain a poly(A) tail, the oligo-dT primers will specifically transcribe mRNA to cDNA. The cDNA strand will subsequently be used as template for the PCR reaction.

![Figure 4](./pics/fig4.png)
*<sub>Figure 4: Schematic representation of  cDNA synthesis. The Oligo-dT primer binds the poly(A) tail of the mRNA. Reverse transcriptase will polymerize the synthesis of the cDNA strand. Source: Wikipedia.org</sub>*

### The principle of PCR 

The PCR technology makes it possible to amplify selected PCR fragments. Two flanking oligonucleotides serve as primers to initiate strand elongation in the 5’ to 3’ direction by DNA polymerase. DNA polymerase will catalyze the incorporation of nucleotides in the growing nucleotide polymer.  

![Figure 5](./pics/fig5.png)
*<sub>Figure 4: Schematic representation of  cDNA synthesis. The Oligo-dT primer binds the poly(A) tail of the mRNA. Reverse transcriptase will polymerize the synthesis of the cDNA strand. Source: Wikipedia.org</sub>*

The DNA polymerases used today are very thermostable. Amplification occurs exponential using cycles of subsequent heating and cooling. At around 95˚C, DNA denatures. Primers can subsequently bind the single stranded DNA at temperatures around 55-60˚C. Thermostable DNA polymerases typically have an optimal temperature around 72˚C. Theoretically, after each cycle, the amount of DNA will be doubled (although in reality the amplification efficiency is often lower). 
The amount of product is thus:

$n_c = n_0*2^c $


Where $n_c$ stands for the number of molecules after a certain number of cycles, $n_0$ stand for the number of input molecules and c stands for the number of cycles. Note that in the third cycle the first product of the desired size appears.

However, the above equation is only valid for the exponential phase. Sooner or later the PCR will enter the plateau phase as primers or nucleotides deplete with each successful amplication round. The PCR reaction typically follows an S-curve (see figure 6). After approximately 30 cycles, the plateau phase will be reached. In most cases, PCR products will be analyzed using agarose gel electrophoresis. The detection is thus an end-point detection. Regardless of the input, the amounts after amplification will be the same. Therefore, regular PCR is not considered a quantitative technique.

![Figure 6](./pics/fig6.png)
*<sub>Figure 6: Typical PCR curve. Source: https://bitesizebio.com/24581/what-is-a-ct-value/</sub>*

### Real-time PCR

Real-time PCR is a specialized PCR technology that uses real-time detection (each cycle). Instead of an end-point detection, real-time PCR makes it possible to follow the amplification after each cycle. In this way, PCR becomes a quantitative technique as the amount of input DNA will influence the PCR curves. This means that real-time PCR can be used to quantify certain DNA sequences such as the amount of viral DNA in blood or the number of transcripts in a sample. Key for real-time PCR is the use of a fluorescence dye that allows detection during synthesis. Often, SYBR Green® is used which binds double stranded DNA (in other words, the newly formed PCR products). As the amount of product increases each cycle, so does the amount of fluorescence. 

![Figure 7](./pics/fig7.png)
*<sub>Figure 7: SYBR Green incorporated in dsDNA. The amount of fluorescence more or less doubles after each cycle. The amount of fluorescence will be measured after each cycle.</sub>*

![Figure 8](./pics/fig8.png)
*<sub>Figure 8: The threshold cycle (CT) is the cycle for which the fluorescence level is higher compared to the threshold value. Source: https://www.sciencedirect.com/science/article/pii/S0098299705000907</sub>*

The $C_T$-value correlates strongly with the starting amount of DNA in the sample. The lower the $C_T$-value, the higher the concentration of DNA in the sample. There is a linear relation between the logarithm of the concentration of DNA and the $C_T$-value. Using a calibration curve, one can reliably quantify the amount of a certain DNA sequence in a sample. 

![Figure 9](./pics/fig9.png)
*<sub>Figure 9: The relationship between the CT-values and the starting amount of template DNA. The amount of starting DNA can be calculated using linear regression analysis.</sub>*

SYBR green binds double stranded DNA regardless of the sequence. This means that aspecific products such as primer dimers will also contribute to the fluorescence signal. In order to discriminate between the correct product and nonspecific products, a melt-curve analysis can be performed. After the PCR reaction, the temperature will be raised slowly. At the $T_M$, 50% of the DNA will be denatured and as a result, the fluorescence level will drop. The $T_M$ is at the inflection point. The first derivative of the graph shows a maximum at this point. Multiple peaks and indicate for aberrant products.

![Figure 10](./pics/fig10.png)
*<sub>Figure 10: Melt-curve analysis. In this case, a single peak is detected indicative for a specific PCR product.</sub>*

### Goal of the experiment:
The goal of this experiment is to investigate if a heat shock changes the expression of the Heat shock protein-encoding mRNA transcript molecules.



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