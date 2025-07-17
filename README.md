**Factorial Design Experiment: Paper Airplane Flight Optimization**
This repository contains a complete factorial design study investigating how the placement of paper clips affects the flight distance of paper airplanes. The project applies principles of statistical experimental design to a hands-on aerodynamic problem and serves as an accessible model for data analysis and linear modeling using R.

**Project Summary**
****Goal****: To determine how clip placement (nose, middle, rear) influences flight distance.
****Design****: Full 2 by 3 factorial design with 3 binary factors and 5 replicates per treatment (total 8×5=40 trials).
****Analysis****: Linear modeling, ANOVA, power analysis, and visualizations conducted in R.
****Outcome****: All three individual placements (nose, middle, rear) significantly impact flight distance. Notably, clips on the nose drastically reduce flight range.


**Methodology**
****Factors****:
Nose: 0 = No clip, 1 = Clip
Middle: 0 = No clip, 1 = Clip
Rear: 0 = No clip, 1 = Clip

****Response Variable****: Flight distance (inches)
****Environment****: Indoor hallway to reduce wind interference

****Tooling****:
- lm() for linear modeling
- anova() for effect testing
- Custom power analysis with power_factorial_23.R
- Plots generated with ggplot2


**Key Findings**
- ****Significant Main Effects****: All three clip positions had statistically significant effects (p < 0.001).
- ****Significant Interaction****: Nose × Middle interaction was significant.
- No Significant Three-Way Interaction.
- Model assumptions (normality, homoscedasticity, independence) were all satisfied.


**Visualization Samples**
Jittered Scatterplot: Explores the impact of each clip position.
Boxplot: Shows variation in flight distance across configurations.
Power Curves: Determines minimum replicates needed for 80% power.

**Files**
****For concision purposes, only the final write-up file is uploaded.****
Paper_Airplanes_Factorial_Design.pdf: Final write-up with complete results and discussion.
Paper_Airplane_Data.csv: Raw dataset with all 40 trials.
power_factorial_23.R: Power analysis helper script.
model_diagnostics.R: Assumption checks and diagnostic plots.

**References**
Ristroph & Wang (2022), Journal of Fluid Mechanics
Swatton (2000), Aircraft Performance Theory for Pilots
Ismail & Ali (2021), Journal of Advanced Research in Fluid Mechanics
Zhang et al. (2020), The Aeronautical Journal

**Applications**
This project is applicable for:
- Teaching factorial design in statistics courses
- Exploring real-world implications of mass distribution in aerospace
- Demonstrating reproducible data analysis in R
