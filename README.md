# Documents Archive

A centralized archive of documents produced from long-running research, engineering, and software projects: papers, theses, technical reports, user manuals, bibliographies, and other written outputs.

This repository contains **documents only**. It does not contain source code, datasets, or build artifacts. Its purpose is to be a single, stable place to find the written outputs of each project, organized by project.

New documents are added over time, so the contents below are grouped by project.

## Projects

| Project | Documents | Topic |
|---------|-----------|-------|
| [Lunar Seismology: Synthetic Moonquakes](#0001-Under-Graduate-lunar-seismology) | 4 | Synthetic lunar accelerograms from Apollo seismic data |

*More projects will be listed here as they are added.*

---

## 0001 Undergraduate Lunar Seismology: Synthetic Moonquakes

Research and software development on **synthetic lunar seismic ground motions (moonquakes)**, carried out at the School of Civil Engineering and Geomatics, Universidad del Valle (Cali, Colombia).

### Documents

| File | Type | Language | Description |
|------|------|----------|-------------|
| `SMGUserManual.pdf` | User manual | English | User manual (v1.0, June 18, 2024) for the *Synthetic Moonquake Generator* (SMG), a MATLAB application that generates synthetic lunar accelerograms and response spectra. Includes GUI description, code review of all source files, compilation steps, installation instructions, and license. |
| `Biblio.bib` | Bibliography | English | BibTeX entry and plain-text citation for the 2020 CONIITI conference paper. |
| *(CONIITI 2020 paper, PDF)* | Conference paper | English | *Preliminary approach to assess the seismic hazard on the Moon*. Overview of the Apollo seismic database tool, probabilistic seismic hazard assessment (PSHA) for shallow moonquakes, and synthetic accelerograms using a Kanai-Tajimi filter with particle swarm optimization. |
| *(Undergraduate thesis, PDF)* | Thesis | Spanish | *Generación de acelerogramas sintéticos para la Luna basados en la metodología de Kanai-Tajimi* (Universidad del Valle, June 2025). Covers Apollo LP record processing, regularized (water-level) deconvolution, PSO-based characterization, and the SMG application. |

> Adjust the file names in the table to match the exact names of the files stored in this repository.

### Background

The Apollo Passive Seismic Experiment (1969-1977) recorded thousands of lunar seismic events, but only a small number of shallow moonquakes are available, and their records are of limited quality. This is a significant obstacle for seismic hazard assessment and structural design of future lunar habitats.

The documents describe a workflow that addresses this gap:

1. **Record processing**: extraction and preprocessing of Apollo long-period (LP) horizontal records from DARTS/JAXA.
2. **Calibration**: instrument-response removal via water-level regularized deconvolution.
3. **Characterization**: fitting a Kanai-Tajimi-type filter and a temporal envelope to each record using particle swarm optimization.
4. **Generation**: producing synthetic moonquake accelerograms and response spectra for three moment-magnitude ranges (2.7-3.2, 3.3-3.6, 3.7-4.1).
5. **Software**: the *Synthetic Moonquake Generator* GUI that automates generation and export of results.

### Suggested Reading Order

1. **CONIITI 2020 paper** for a short overview of the motivation and approach.
2. **Thesis** for the full methodology, validation, and results.
3. **SMG User Manual** to use the software or understand its implementation.
4. **`Biblio.bib`** for citing the work.

### Citing

For the conference paper:

```bibtex
@INPROCEEDINGS{9240257,
  author={Cadena, Paula and Ruiz, Santiago and Arcila, Oscar and Prado, Vanessa and Patiño, Andres and Gómez, Daniel and Cruz, Alejandro and Ospina, Lina and Gómez, Isabel},
  booktitle={2020 Congreso Internacional de Innovación y Tendencias en Ingeniería (CONIITI)},
  title={Preliminary approach to assess the seismic hazard on the Moon},
  year={2020},
  pages={1-6},
  doi={10.1109/CONIITI51147.2020.9240257}
}
```

For the thesis:

> Arcila Giraldo, O. A. (2025). *Generación de acelerogramas sintéticos para la Luna basados en la metodología de Kanai-Tajimi* [Undergraduate thesis]. Universidad del Valle, Santiago de Cali, Colombia.

For the software manual:

> Arcila, O., Gómez, D., & Cruz, A. (2024). *Synthetic Moonquake Generator User Manual, Version 1.0*. Universidad del Valle.

### Credits

- **Oscar Arcila**: author of the thesis and main developer of the SMG software.
- **Daniel Gómez** and **Alejandro Cruz**: thesis co-directors and SMG co-authors.
- Additional authors of the CONIITI 2020 paper are listed in `Biblio.bib`.

Research funded by the Universidad del Valle internal call project *Metodología para la caracterización de la amenaza sísmica, generación de sismos sintéticos y espectros de diseño para la Luna* (21078). Apollo seismic data were obtained from the Data ARchives and Transmission System (DARTS), provided by C-SODA at ISAS/JAXA.

---

## Licensing and Usage Notes

Each document keeps its own license or publisher terms. Please verify them before reusing or redistributing anything from this repository. Known cases:

- **SMG User Manual**: [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). It includes unmodified third-party code (*Image Mouse Zoom and Pan*, Dany Cabrera, CC BY-SA 3.0).
- **CONIITI 2020 paper**: © IEEE; consult the publisher's terms.
- **Thesis**: subject to the policies of Universidad del Valle.

This repository does not grant rights beyond those set by the original licenses.

## Repository Structure

Documents are grouped in one folder per project once the archive grows beyond a handful of files. Suggested layout:

```
.
├── README.md
├── 0001-Under-Graduate-lunar-seismology/
│   ├── Biblio.bib
│   ├── SMGUserManual.pdf
│   ├── <CONIITI 2020 paper>.pdf
│   └── <Thesis>.pdf
└── <future-project>/
    └── ...
```
