# Fdataset

Fdataset is a benchmark dataset widely used for Drug–Disease Association (DDA) prediction and drug repositioning research.

## Dataset Information

| Item | Value |
|--------|--------|
| Drugs | 593 |
| Diseases | 313 |
| Known Drug–Disease Associations | 1933 |
| Drug Similarity Matrix | 593 × 593 |
| Disease Similarity Matrix | 313 × 313 |
| Association Matrix | 593 × 313 |

The dataset was originally introduced in the HNRD framework by Wang et al. and has been adopted by numerous DDA prediction studies.

## Files

### drug_sim.csv

Drug structural similarity matrix.

Shape:

```text
593 × 593
```

Each row and column corresponds to a drug.

---

### disease_sim.csv

Disease semantic similarity matrix.

Shape:

```text
313 × 313
```

Each row and column corresponds to a disease.

---

### assoc.csv

Known drug–disease association matrix.

Shape:

```text
593 × 313
```

Values:

- 1 = known association
- 0 = unknown association

Rows correspond to drugs and columns correspond to diseases.

---

### drug.txt

List of drug names or DrugBank IDs corresponding to rows of the matrices.

---

### disease.txt

List of disease names or OMIM IDs corresponding to columns of the matrices.

## Data Sources

### Drug Information

DrugBank

https://go.drugbank.com

### Disease Information

OMIM (Online Mendelian Inheritance in Man)

https://www.omim.org

### Drug–Disease Associations

Comparative Toxicogenomics Database (CTD)

http://ctdbase.org

## Common Usage

This dataset is frequently used for:

- Drug Repositioning
- Drug–Disease Association Prediction
- Graph Neural Networks (GNN)
- Graph Contrastive Learning
- Heterogeneous Graph Learning
- Matrix Factorization Methods

## Citation

If you use this dataset, please cite the original works:

```bibtex
@article{Wang2019DrugDiseaseAP,
  title={Drug-Disease Association Prediction Based on Neighborhood Information Aggregation in Neural Networks},
  author={Yingdong Wang and Gaoshan Deng and Nianyin Zeng and Xiao Song and Yuanying Zhuang},
  journal={IEEE Access},
  year={2019},
  volume={7},
  pages={50581-50587},
  url={https://api.semanticscholar.org/CorpusID:133606089}
}
```

## Related Studies

- PREDICT
- LRSSL
- HNRD
- NTSIM
- DRRS
- HGCL-DR
- SMGCL
- HINGRL
- HGAT-CL

## License

This repository is intended for academic and research purposes only.
Users should follow the original licenses and terms of the corresponding data sources.
