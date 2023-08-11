# ESM-NBR
The data, supplementary information and standalone program of ESM-NBR.
# Pre-requisite:
- Python(3), numpy, pytorch, esm(https://github.com/facebookresearch/esm)
- Linux system (suggested CentOS 7)
 # Running
 ```
#
 $ python prediction.py your_fasta_path device save_dir model_type split_len dna_threshold rna_threshold
```
-your_fasta_path: pth of input protein sequences in fasta format. (support multi sequence)
-device: cpu or cuda
-save_dir: The directory where the results are generated
-model_type: YK17 or DRNA1068
-split_len: Long sequences are cut into short sequences to generate ESM feature representations.
-dna_threshold: 0.8 is recommended.
-rna_threshold: 0.1 is recommended.

# Reference
[1] Wenwu Zeng, Dafeng Lv, and Shaoliang Peng. ESM-NBR: fast and accurate nucleic acid-binding residue prediction via protein language model feature representation and multi-task learning. Submitted.
