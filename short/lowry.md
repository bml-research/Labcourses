![Hanze](../hanze/hanze.png)

[Back to the home page of the crash course](./short.md)

# The Lowry Assay

## Learning outcomes
- Weighing chemicals
- Pipetting fluids
- Designing a standard curve
- Performing absorption measurements after a chemical reaction
- Applying second order regression using a spreadsheet
- Using the ABC formula to calculate the protein concentration

## Introduction
The Lowry assay (1951) is an often-cited, generally used protein assay. The modified Lowry is done entirely at room temperature which makes it easy to use for practical courses.

## Principle 
Under alkaline conditions the divalent copper ion ($Cu^{2+}$) forms a complex with peptide bonds in which it is reduced to a monovalent ion ($Cu^{+}$). Monovalent copper ions and the radical groups of some aminon acids in protein (tyrosine, tryptophan, and cysteine) react with Folin reagent to produce an unstable product that becomes reduced to molybdenum/tungsten blue. The end product gives a specific absorbance at 750 nm. Proteins with an abnormally high or low percentage of tyrosine, tryptophan, or cysteine residues will give high or low errors, respectively.

$Protein + Cu^{2+} \rightarrow Protein - Cu^+_{complex} + Folin_{reagens} \rightarrow blue-product$

## Preparation of the reagents 
1.	Dissolve 20 gr sodium carbonate in 260 ml water, 0.2 gr cupric sulfate (5x hydrated) in 20 ml water, and 0.4 gr sodium potassium tartrate tetrahydrate in 20 ml water.  Prepare the solutions separately until obtaining a clear solution. Mix all three solutions to prepare the __copper reagent__. (_This solution will be prepared by the teacher_)
2.	Prepare 10 ml of a 1% (w/v) solution of sodium dodecyl sulfate (SDS). 
3.	Prepare 10 ml of a 1 mol/L solution of NaOH. 
4.	For the __2x Lowry concentrate__ mix 3 parts copper reagent with 1 part SDS and 1 part NaOH. The solution stays stable for 2-3 weeks. Warm the solution up to 37°C if a white precipitate forms, and discard if there is a black precipitate. Better, keep the three stock solutions, and mix just before use (calculate the expected volume needed based on the number of assays performed) 
5.	Prepare __0.2 M Folin reagent__ by mixing 1 ml 2 M Folin reagent with 9 ml water. Kept in an amber bottle (or tube in Aluminum foil), the dilution stays stable for several months. 

## Assay 
Prepare in duplicates:
1.	Dilute the unknown samples to an estimated 0.025-0.25 mg/ml with demi-water. If the concentration can't be estimated it is advisable to prepare a range of 2-3 dilutions spanning an order of magnitude. Prepare 400 microliters each dilution. 
2.	Prepare a reference blank of 400 microliters demi-water. Prepare standards from 0.025 up to 0.25 mg/ml bovine serum albumin. (this will be used for the calibration curve)
3.	Add 400 microliters of 2x Lowry concentrate, mix thoroughly, incubate at room temp. 10 min. 
4.	Add 200 microliters 0.2 M Folin reagent very quickly, and vortex immediately. Complete mixing of the reagent must be accomplished quickly to avoid decomposition of the reagent before it reacts with protein. Incubate for 30 min. more at room temperature. 
5.	Use polystyrene cuvettes to read the absorbance at 750 nm.
6.	Determine the protein concentration of the samples by using the calibration curve performed with the standard bovine serum albumin. See the next session.

## Processing lab data using a spreadsheet

- Plot the OD values as a function of the protein concentration. The Beer–Lambert law predicts a linear relationship between the protein concentration and the optical density. However, it is well known that the Lowry method yields a second degree polynomial line. Include correct axis titles for your graph.
- Perform a second order regression on your data using Microsoft Excel:

![Lowry Example](./lowry/lowry.png)


- Set up the second order regression equation model as $y = ax^2 + bx + c$
- Fill in your y-value and set the equation to 0.
- Use the ABC formula to calculate the protein concentration in your sample. ABC-formula: $x = \frac{-b\ \pm\ \sqrt{b^2 - 4ac}}{2a}$
- If all went well, you will end up with two results for x. Which of the two results is correct?
- Report the protein concentration in your lab journal.

The end...

[Back to the home page of the crash course](./short.md)

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