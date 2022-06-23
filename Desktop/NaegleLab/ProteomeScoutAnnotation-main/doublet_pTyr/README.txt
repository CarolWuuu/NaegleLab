To generate the tkr_bcr_tcr.csv, complete the following steps:
1. Generate a list of protein ID with search term family:tyr protein kinase AND organism:“Homo sapiens (Human) [9606]” in Uniprot. A generated list of tyr_kinase_human.txt is located in 
2. Manually generate a list of ID of B cell signaling receptors by looking for their ID in Uniprot. A generated list of bcr.txt is located in . BCR included in this list are listed below:
	▪	CD21
	▪	CD19
	▪	CD81
	▪	LEU13(IFITMI)
	▪	FCGR2B
	▪	IgD, IgM
	▪	CD72
	▪	CD22
	▪	CD79A (Ig-alpha), CD79B (Ig-beta)
3. Manually geneate a list of ID of T cell signaling receptors. A generated list of tcr.txt is located in . TCR included in this list are listed below:
	▪	CD28
	▪	ICOS
	▪	CD40L
	▪	CD3E
	▪	CD3D
	▪	CD3G
	▪	CD4
	▪	CD8
	▪	CD45 (PTPRC)
	▪	CTLA4
	▪	PD-1
4. Append tcr.txt and bcr.txt to tyr_kinase_human.txt. An extended list of tyr_kinase_human_bcr_tcr_June21_2022.txt located on https://github.com/NaegleLab/ProteomeScoutAnnotation/tree/main/Data/Proteome.
5. Run create_df.py located on https://github.com/NaegleLab/ProteomeScoutAnnotation/tree/main/doublet_pTyr with the protein ID list tyr_kinase_human_bcr_tcr_June21_2022.txt 
Note: create_df.py used bivalent.py as a module