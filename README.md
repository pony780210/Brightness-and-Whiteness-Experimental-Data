# Brightness and Whiteness Experimental Data

This repository contains psychophysical data on how observers perceive the brightness and white point of an automotive head-up display (HUD) as they adapt to changes in ambient lighting. The Brightness Experiment records perceived brightness ratings at three display stimulus levels. The Whiteness Experiment records binary choices used to estimate the perceived white point in two main experiments.

## Data files

| Experiment | Excel workbook | Data rows | Participant columns |
| --- | --- | ---: | ---: |
| Brightness | [final_result.xlsx](Brightness%20Experiment/final_result.xlsx) | 1,440 | 20 |
| Whiteness, Main Experiment 1 | [final_result_exp2-1.xlsx](Whiteness%20Experiment/Main%20Experiment%201/final_result_exp2-1.xlsx) | 2,160 | 12 |
| Whiteness, Main Experiment 2 | [final_result_exp2-2.xlsx](Whiteness%20Experiment/Main%20Experiment%202/final_result_exp2-2.xlsx) | 2,160 | 12 |

Each workbook contains one worksheet. Row counts exclude the header.

## Ambient lighting conditions

Ambient illuminance is given in lux (lx), and correlated color temperature (CCT) is given in kelvin (K). The two digits in a transition code identify the initial and subsequent lighting conditions in order. For example, code `13` denotes a transition from F1 to F3.

| Condition | Ambient illuminance (lx) | Ambient CCT (K) |
| --- | ---: | ---: |
| F1 | 2,500 | 3,000 |
| F2 | 2,500 | 6,500 |
| F3 | 800 | 3,000 |
| F4 | 800 | 6,500 |
| F5 | 100 | 3,000 |
| F6 | 100 | 6,500 |

## Brightness Experiment

- **Column A** contains the lighting transition code at the start of each 180-row block. The following blank cells in column A belong to that same block.
- **Column B** contains the display stimulus level code. The repeating sequence `64`, `128`, and `256` corresponds to the low, medium, and high stimulus levels, respectively. These values are stimulus codes.
- **Columns C–V** contain perceived brightness ratings from participants `01` through `20`. The rating scale used the medium-luminance reference stimulus as 50 and black as 0.
- **Column W (`avg`)** contains the arithmetic mean of all 20 participant ratings for each row. To reproduce an analysis based on a subset of participants, compute the mean from the relevant participant columns.
- Each transition block contains 60 consecutive sets of three stimulus levels in recording order. The lighting transition occurred 300 s into the rating sequence, with ratings collected at 10 s intervals over 5 min before and 5 min after the transition.

## Whiteness Experiment

- **Column A** contains the lighting transition code at the start of each 360-row block. The following blank cells in column A belong to that same block. This column is labeled `Block_Group` in Main Experiment 1.
- **Column B** contains the repeating stimulus condition codes `1` through `6`. This column is labeled `Condition` in Main Experiment 1.
- **Columns C–N** contain binary responses (`0` or `1`) under participant IDs. Preserve the binary coding when importing the data and consult the study methods for the response coding and stimulus definitions used to estimate the white point.
- The two workbooks list different participant IDs. All participant response cells in both workbooks contain a recorded binary value (`0` or `1`).

## Access and citation

Download the Excel files using the links above or download the full repository from the [GitHub repository page](https://github.com/pony780210/Brightness-and-Whiteness-Experimental-Data) using **Code → Download ZIP**. If you use the data, cite this repository and the associated manuscript when available. Include the commit identifier for the version of the data you used.
