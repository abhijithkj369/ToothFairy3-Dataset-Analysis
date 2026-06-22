# ToothFairy3 Dataset Analysis

Comprehensive exploratory data analysis (EDA) and statistical assessment of the ToothFairy3 dental CBCT segmentation dataset.

This repository provides tools for analyzing label distributions, anatomical structure frequencies, class imbalance, canal statistics, tooth occurrence patterns, and generating publication-quality figures and tables for research papers.

---

## Dataset

This project analyzes the ToothFairy3 dataset, a large-scale dental CBCT segmentation benchmark containing:

* 532 CBCT volumes
* 77 semantic classes
* 76 foreground anatomical labels
* 32 tooth labels
* 32 tooth pulp labels
* Jaw bones, canals, sinuses, airway, restorations, and dental structures

Official Dataset:

https://ditto.ing.unimore.it/toothfairy3/

---

## Anatomical Structures

### Jaw Bones

* Lower Jawbone (Mandible)
* Upper Jawbone (Maxilla)

### Canal Structures

* Left Inferior Alveolar Canal
* Right Inferior Alveolar Canal
* Left Mandibular Incisive Canal
* Right Mandibular Incisive Canal
* Lingual Canal

### Sinuses

* Left Maxillary Sinus
* Right Maxillary Sinus

### Airway

* Pharynx

### Dental Restorations

* Bridge
* Crown
* Implant

### Teeth

32 individual teeth following the FDI numbering system.

### Tooth Pulps

32 corresponding pulp cavity labels.

---

## Analysis Performed

### Label Frequency Analysis

Computes:

* Number of cases containing each label
* Label occurrence percentage
* Rare structure identification

### Class Imbalance Analysis

Computes:

* Total voxel counts
* Mean voxel counts
* Median voxel counts
* Minimum voxel counts
* Maximum voxel counts

Useful for understanding segmentation difficulty and long-tail label distributions.

### Anatomical Category Analysis

Structures are grouped into:

* Bones
* Canals
* Sinuses
* Airway
* Restorations
* Teeth
* Pulps

### Canal Analysis

Evaluates:

* Inferior Alveolar Canals
* Mandibular Incisive Canals
* Lingual Canal

Including left-right anatomical comparisons.

### Publication-Quality Visualization

Automatically generates:

* Label frequency plots
* Class imbalance plots
* Category distribution charts
* Canal comparison figures

---

## Repository Structure

```text
.
├── notebooks/
│   └── ToothFairy3_Analysis.ipynb
│
├── results/
│   ├── ToothFairy3_Label_Analysis.xlsx
│   ├── Figure1_Label_Frequency.png
│   ├── Figure2_Class_Imbalance.png
│   ├── Figure3_Category_Distribution.png
│   ├── Figure4_Canal_Comparison.png
│   └── ToothFairy3_Publication_Report.xlsx
│
├── README.md
└── requirements.txt
```

---

## Installation

```bash
git clone https://github.com/yourusername/ToothFairy3-Dataset-Analysis.git

cd ToothFairy3-Dataset-Analysis

pip install -r requirements.txt
```

---

## Requirements

```text
pandas
numpy
matplotlib
openpyxl
jupyter
```

Install:

```bash
pip install pandas numpy matplotlib openpyxl jupyter
```

---

## Usage

Place the generated analysis Excel file:

```text
ToothFairy3_Label_Analysis.xlsx
```

inside the project directory.

Open:

```bash
jupyter notebook
```

Run:

```text
ToothFairy3_Analysis.ipynb
```

The notebook will automatically generate:

* Publication tables
* Statistical summaries
* Research figures
* Excel reports

---

## Example Outputs

### Figure 1

Label Frequency Distribution

Shows how frequently each anatomical structure appears across the 532 CBCT scans.

### Figure 2

Class Imbalance Analysis

Visualizes the voxel distribution of anatomical structures using a logarithmic scale.

### Figure 3

Category Composition

Displays the proportion of teeth, pulps, bones, canals, sinuses, airway structures, and restorations.

### Figure 4

Canal Comparison

Compares the relative sizes and occurrence frequencies of dental canal structures.

---

## Applications

This analysis can be used for:

* Dataset understanding
* Medical image segmentation research
* Class imbalance assessment
* Model design decisions
* Benchmark reporting
* Scientific publications

---

## Citation

If you use ToothFairy3, please cite the original dataset authors.

---

## License

This repository only provides dataset analysis tools.

Please refer to the official ToothFairy3 dataset license and terms of use before downloading or redistributing dataset content.
