# Cytoskeleton (BBBC018-19465)

## Student Information

- **Student ID:** 202400765
- **Chosen Phenotype:** Actin dots
- **Image Field ID:** 19465
- **Actin Image:** `19465-actin.DIB`
- **DNA Image:** `19465-DNA.DIB`
- **pH3 Image:** `19465-pH3.DIB`

## Introduction

This activity focused on observing cell morphology and fluorescence staining patterns using the BBBC018v1 image dataset. Fiji/ImageJ was used to examine the images and measure five selected cells. The collected data were then analyzed in RStudio to calculate descriptive statistics and create graphs showing cell area, circularity, and actin fluorescence intensity.

## Software and Dataset

- **Fiji/ImageJ** - image visualization and cell measurements.
- **RStudio and R** - data analysis and visualization.
- **GitHub** - organizing and presenting the project files.


## Dataset

The BBBC018 dataset contains fluorescence images of HT29 human colon cancer cells. In this activity, the images were analyzed to examine cell morphology and identify F-actin staining patterns.

**BBBC018 download link:** https://bbbc.broadinstitute.org/BBBC018

# Procedures
<img width="620" height="418" alt="image" src="https://github.com/user-attachments/assets/364ae8b3-af76-4d3d-bfd5-75d97dcff621" />

*Figure 1. The Fiji download page where it shows the available versions; Windows x86-64 version was selected for installation.*

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/8827dbe8-df7b-4e1d-b2f7-9bb384a1daf6" />

*Figure 2. Dowloaded and extracted dataset of BBBC018.*

# Opening of the Selected Image on Fiji

The selected actin image, `19465-actin.DIB`, was opened in Fiji to measure cell morphology. The DNA and pH3 images were also viewed as references. The image files were opened using the Bio-Formats Importer.

<img width="1365" height="767" alt="Screenshot 2026-10-28 085016" src="https://github.com/user-attachments/assets/762e4769-442c-4f8f-abe8-405ce043c017" />
<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/de9bbf44-d5bc-4838-a57c-ace339ff433f" />
<img width="609" height="402" alt="Screenshot 2026-10-28 085150" src="https://github.com/user-attachments/assets/608c90f7-bcd9-4cbd-8143-959b8adfb730" />

*Figure 3. A step by step guide on opening the selected fluorescence image in the Fiji app.*

# Selecting/Measuring/Tracing the selected five cells

Five clearly visible cells were chosen from the actin image and outlined using Fiji’s selection tools. The selected cells were organized in the ROI Manager, and their area, mean fluorescence intensity, circularity, and aspect ratio were measured. The measurement results were then exported and saved as `fiji_results.csv`.

<img width="1055" height="617" alt="image" src="https://github.com/user-attachments/assets/f3b6ab35-4049-42fb-aef9-e226aae9645d" />

*Figure 3. Selected cells, ROIs, Measuring it in  Fiji.*

# Analyzation using R-studio

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/a38d8189-ffd6-4b0c-897f-20e55bc50a69" />

*Figure 4. Data Analyzation in R-studio.*


# Results 
| Phenotype | Image ID | Cells Measured | Mean Area (px²) | Mean Circularity | Mean Aspect Ratio | Mean Actin Signal |
|---|---:|---:|---:|---:|---:|---:|
| Actin dots | 19465 | 5 | 258.2 | 0.8476 | 1.0922 | 1212.8878 |

The results show that the five selected (19465) cells had generally rounded shapes and similar dimensions. The mean actin fluorescence intensity was 1212.8878.

# Plots Result in R-studio

<img width="900" height="650" alt="actin_intensity" src="https://github.com/user-attachments/assets/0c63e7d7-9e97-4bc1-84ac-df20f80b55bf" />

The graph shows that Cell 1 had the highest actin fluorescence intensity, followed by Cells 3 and 2. Cell 4 had the lowest intensity, while Cell 5 showed a moderate signal. These differences indicate variation in actin fluorescence intensity among the five selected cells.

<img width="900" height="650" alt="area_vs_circularity" src="https://github.com/user-attachments/assets/43c86882-a800-4f70-af4c-998c33750880" />

The graph shows the relationship between cell area and circularity for five selected cells. Cell 5 had the highest circularity despite having the smallest area, while Cell 3 had the lowest circularity. Cell 1 had the largest area and relatively high circularity. Overall, the cells varied in size and shape, suggesting differences in their morphology.


# Guide Questions

**1. Which specific phenotype did you choose, and what visible features support that choice?**

I chose the Actin dots phenotype because the actin fluorescence image showed visible dot-like patterns in the selected regions.

**2. Were your five cells mostly round or elongated? Refer to your circularity and aspect-ratio results.**

The five cells were generally rounded, with a mean circularity of 0.8476 and a mean aspect ratio of 1.0922. These values suggest that the cells were relatively round and had similar length and width.

**3. What role does actin play in maintaining cell shape and in cell movement (Karp Chapter 9)?**

Actin helps maintain cell shape by forming part of the cytoskeleton beneath the cell membrane. It also supports cell movement by reorganizing its filaments and generating forces that help the cell move.

**4. Why can a single fixed fluorescence image NOT show how fast a cell moves?**

A single fixed fluorescence image captures the cell at only one point in time. Measuring cell movement requires images taken at different time points to track changes in cell position.



