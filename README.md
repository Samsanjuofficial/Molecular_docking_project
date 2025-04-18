# Molecular Docking of Annona muricata Compounds Against FabH Protein

This project explores the binding potential of various phytochemicals derived from *Annona muricata* against the FabH protein, an antibacterial target. Molecular docking was performed and results were compared with the standard drug, ciprofloxacin.

## **Objective**
To identify potential natural antibacterial agents by docking bioactive compounds from *Annona muricata* against the FabH protein and compare their affinities with ciprofloxacin.

## **Tools Used**
- **AutoDock Vina** (via PyRx) – for molecular docking
- **PyRx** – for ligand preparation and docking
- **Discovery Studio** – for visualization
- **SwissADME / ADMET tools** – for pharmacokinetic property prediction

## **Target Protein**
- **FabH (β-ketoacyl-ACP synthase III)**
- Protein downloaded from RCSB PDB and prepared using AutoDock Tools (converted to .pdbqt)

## **Ligands**
- Various phytochemicals from *Annona muricata*
- Structures retrieved from PubChem and converted to .pdbqt via PyRx
- Standard reference: **Ciprofloxacin**

## **Key Results**
| Compound        | Binding Affinity (kcal/mol) | Notes                            |
|-----------------|-----------------------------|----------------------------------|
| Liriodenine     | -9.1                        | Higher affinity than ciprofloxacin |
| Annomuricin A   | -8.3                        | Moderate binding                 |
| Annopentocin    | -8.0                        | Moderate binding                 |
| Ciprofloxacin   | -7.6                        | Reference drug                   |

**Liriodenine** showed the highest binding affinity against FabH, suggesting strong potential as a natural antibacterial agent.

## **Visualizations**
Docking poses and binding interactions were visualized using Discovery Studio.

![Binding pose of Liriodenine](images/liriodenine_binding.png)

## **ADMET Analysis**
All selected ligands were analyzed using SwissADME and admetSAR to evaluate:
- Lipinski's Rule of Five
- Gastrointestinal absorption
- Blood-brain barrier penetration
- Toxicity profile

## **Conclusion**
Liriodenine from *Annona muricata* shows strong binding affinity and favorable ADMET properties, suggesting its potential as a lead compound for antibacterial drug development targeting FabH.

---

## **How to Use This Repo**
1. Clone or download this repository
2. View docking files in `docking_results/`
3. Use PyRx or AutoDock Tools to replicate the docking
4. Refer to `ADMET_reports/` for pharmacokinetic analysis

---

**Author:** sanjay.s  
**License:** MIT
