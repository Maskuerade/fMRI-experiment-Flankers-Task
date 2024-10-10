# fMRI Flanker Task Experiment: Neuroscience Project

## Overview

This project is an fMRI analysis of the Flanker task, designed to investigate cognitive control and response inhibition. The dataset used comes from a standard Flanker task, which involves participants responding to a central stimulus while ignoring flanking distractors. The project aims to analyze neural activity related to these cognitive processes using functional magnetic resonance imaging (fMRI) data.

The analysis pipeline and scripts in this repository rely on Andy's Brain Book, a comprehensive resource for fMRI data analysis: [Andy's Brain Book](https://andysbrainbook.readthedocs.io/en/latest/).

## Objective

- Investigate brain regions activated during the Flanker task.
- Explore how interference from distractors affects neural activation.
- Understand cognitive control mechanisms involved in resolving conflict.

## Dataset

The Flanker dataset used in this project contains fMRI data collected from participants performing the Flanker task. The task includes trials where participants must respond to a central target, while the surrounding flanker stimuli are either congruent or incongruent with the target. This dataset helps to isolate neural correlates of interference control.

## Project Structure

```
.
├── data/                      # Contains raw and preprocessed fMRI data
├── scripts/                   # Python scripts for data analysis and processing
│   ├── preprocessing.py       # Preprocessing steps: motion correction, slice timing correction, etc.
│   ├── analysis.py            # Statistical analysis of fMRI data
│   ├── glm_analysis.py        # General Linear Model (GLM) analysis
│   └── visualization.py       # Visualization of activation maps and results
├── notebooks/                 # Jupyter notebooks for step-by-step analyses
├── README.md                  # Project documentation (this file)
└── requirements.txt           # Python dependencies
```

## Analysis Pipeline

1. **Preprocessing**:  
   The preprocessing of the fMRI data follows steps outlined in Andy's Brain Book, including:
   - Motion correction
   - Slice-timing correction
   - Spatial normalization
   - Smoothing

2. **General Linear Model (GLM)**:  
   A GLM is applied to the preprocessed fMRI data to model the relationship between brain activity and task conditions (congruent vs. incongruent trials). This step estimates the brain regions associated with cognitive control and response inhibition.

3. **Statistical Analysis**:  
   Statistical maps are generated to examine areas of significant activation for congruent and incongruent conditions, focusing on regions such as the anterior cingulate cortex (ACC) and prefrontal cortex (PFC).

4. **Visualization**:  
   Results are visualized using activation maps and plots to interpret the brain regions engaged during the task. The visualization script produces brain overlays that display regions activated during the Flanker task.

## Resources

For a step-by-step guide and in-depth explanation of fMRI data analysis techniques, refer to [Andy's Brain Book](https://andysbrainbook.readthedocs.io/en/latest/), which provides tutorials and code examples for working with fMRI data.

## Contributing

Contributions to improve the project, whether in the form of bug fixes, new analysis features, or documentation updates, are welcome! Please submit pull requests or open issues for any suggestions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

We would like to thank Andy's Brain Book for providing accessible and detailed tutorials on fMRI data analysis, which served as the foundation for this project.

---

Feel free to customize the README as you see fit!
