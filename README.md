# molecular-networking-assignment
Assignment for GNPS molecular networking tutorial
# 🧪 GNPS Molecular Networking Report

## 🔗 Task Overview

This project performs a molecular networking analysis using the GNPS platform. The task includes:

1. Generating a molecular network
2. Exploring a molecular family using **neutral losses**
3. Comparing MS/MS spectra of two connected compounds
4. Uploading results and documentation to GitHub

---

## ✅ Step 1: Generate a Molecular Network

A classical molecular networking workflow was run on GNPS using MS/MS data.

- **GNPS Job Link**:  
  [https://gnps.ucsd.edu/ProteoSAFe/status.jsp?task=72fc2b92d3ca456891d7297b5f0e9a05](https://gnps.ucsd.edu/ProteoSAFe/status.jsp?task=72fc2b92d3ca456891d7297b5f0e9a05)

- **Interactive Network Viewer**:  
  [View Network](https://gnps.ucsd.edu/ProteoSAFe/result.jsp?view=network_displayer&componentindex=8&highlight_node=926&task=72fc2b92d3ca456891d7297b5f0e9a05)

---

## ✅ Step 2: Explore a Molecular Family with Neutral Losses

- Node **926** was selected as a reference compound.
- A connected node, **1048**, showed a strong spectral similarity.
- Using the **`edgeannot`** feature, the edge between nodes 926 and 1048 was annotated with a **neutral loss of CH₄ (16 Da)**.
- This suggests a structural modification such as demethylation within the compound family.

> This confirms the exploration of a molecular family through shared neutral loss behavior.

---

## ✅ Step 3: Compare MS/MS Spectra

The spectra of **Node 926** and **Node 1048** were compared using GNPS’s “Compare MS²” tool.

### Figure 1: MS/MS Spectra Comparison

The comparison reveals:

- Shared major fragment peaks
- A neutral loss of CH₄ between specific ions
- High spectral alignment score (cosine > 0.7)

![Spectral Comparison](figures/spectrum_comparison.png)

---

## ✅ Step 4: Upload to GitHub

All relevant files and documentation were uploaded to this GitHub repository, including:

- GNPS job links
- README documentation
- MS/MS comparison image

---

## ⚙️ GNPS Parameters Summary

| Parameter                      | Value           |
|-------------------------------|-----------------|
| Workflow                      | Classical Molecular Networking |
| Precursor Mass Tolerance      | 0.02 Da         |
| Fragment Ion Mass Tolerance   | 0.02 Da         |
| Cosine Score Threshold        | 0.7             |
| Minimum Matched Peaks         | 6               |
| Network TopK                  | 10              |
| Minimum Cluster Size          | 1               |
| Library Search                | Enabled         |
| Analog Search                 | Enabled         |
| Include Neutral Losses        | ✅ Yes          |
| Edge Annotation               | ✅ Enabled (`edgeannot`) |

