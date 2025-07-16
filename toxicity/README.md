# Toxicity Prediction

Although there are many datasets you could consider using for toxicity prediction, a famous one is the [`Tox21`dataset](https://tripod.nih.gov/tox21/challenge/data.jsp)

This version of Tox21 is from a website called [MoleculeNet](https://moleculenet.org/).

The columns in the included CSV files indicate activity for he twelve Tox21 assays. These assays are lab screens that ask: Does this compound turn on (or otherwise perturb) a specific cellular pathway or receptor? Each column reports the result for one assay: 1 = active, 0 = inactive, blank = not tested.

If something is 1, we’ll label it “toxic (hit)” for that assay in class because the compound activated (or otherwise perturbed) the pathway that assay is designed to detect. In toxicology, such pathway hits are mechanistic warning signs: they suggest the compound could contribute to adverse effects if similar activity occurs in a whole organism at relevant exposures.

| Column            | Group            | Meaning                                                      | Values    |
| ----------------- | ---------------- | ------------------------------------------------------------ | --------- |
| **NR-AR**         | Nuclear Receptor | Androgen Receptor full‑length assay                          | 0/1/blank |
| **NR-AR-LBD**     | Nuclear Receptor | AR Ligand Binding Domain assay                               | 0/1/blank |
| **NR-AhR**        | Nuclear Receptor | Aryl hydrocarbon Receptor                                    | 0/1/blank |
| **NR-Aromatase**  | Nuclear Receptor | Aromatase (CYP19)                                            | 0/1/blank |
| **NR-ER**         | Nuclear Receptor | Estrogen Receptor full‑length                                | 0/1/blank |
| **NR-ER-LBD**     | Nuclear Receptor | ER Ligand Binding Domain                                     | 0/1/blank |
| **NR-PPAR-gamma** | Nuclear Receptor | PPAR‑γ                                                       | 0/1/blank |
| **SR-ARE**        | Stress Response  | Antioxidant response element                                 | 0/1/blank |
| **SR-ATAD5**      | Stress Response  | ATAD5 genotoxicity                                           | 0/1/blank |
| **SR-HSE**        | Stress Response  | Heat shock factor response element                           | 0/1/blank |
| **SR-MMP**        | Stress Response  | Mitochondrial membrane potential                             | 0/1/blank |
| **SR-p53**        | Stress Response  | p53 tumor suppressor pathway                                 | 0/1/blank |
| **mol\_id**       | Metadata         | Molecule identifier (e.g., `TOX3021`)                        | string    |
| **smiles**        | Structure        | Canonical (or near‑canonical) SMILES string for the compound | string    |
