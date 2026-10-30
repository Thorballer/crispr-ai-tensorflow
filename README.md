# CRISPR AI — TensorFlow research prototype

A sequence-to-sequence research prototype conditioning on sequence data and effect descriptions to predict mutation-change tokens, with related protein/text experiments.

## Project status

Historical notebooks from Daniel Goldberg’s Kaggle account, organized for a maker portfolio. The model code is preserved, not rewritten during packaging. See [PROVENANCE.json](PROVENANCE.json) for original notebook URLs, timestamps, and SHA-256 hashes.

## Notebooks

- [science-fair-gene-mutation.ipynb](notebooks/science-fair-gene-mutation.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-gene-mutation)
- [tokenizer-dna-mutations.ipynb](notebooks/tokenizer-dna-mutations.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/tokenizer-dna-mutations)
- [gene-dataset.ipynb](notebooks/gene-dataset.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/gene-dataset)
- [science-fair-function-to-protein.ipynb](notebooks/science-fair-function-to-protein.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-function-to-protein)
- [science-fair-protein-to-process.ipynb](notebooks/science-fair-protein-to-process.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-protein-to-process)

## Running

Use the original Kaggle environment where possible: open the source notebook, attach its declared datasets/models, select the hardware expected by its setup cells, and run cells in order. Inspect any install, account-login, upload, or filesystem-changing cells before executing them.

For a local adaptation, install the packages listed in `requirements.txt` in an isolated environment and adjust `/kaggle/input` paths. Those packages are inferred from imports, **not** a tested lockfile. Historical APIs and accelerator assumptions can require changes. Do not run all training notebooks at once.

### Referenced Kaggle datasets

- [thorballer/all-uniprot-isodata](https://www.kaggle.com/datasets/thorballer/all-uniprot-isodata)
- [thorballer/full-unlinked-mutations-ds](https://www.kaggle.com/datasets/thorballer/full-unlinked-mutations-ds)
- [thorballer/human-protein-dataset](https://www.kaggle.com/datasets/thorballer/human-protein-dataset)
- [thorballer/parsed-dna-mutations](https://www.kaggle.com/datasets/thorballer/parsed-dna-mutations)

### Referenced Kaggle models/tokenizers

- `thorballer/dna-mutations-tokenizers/TensorFlow2/default/4`
- `thorballer/protein_ai_tokenizers/TensorFlow2/default/1`
- `thorballer/protein_ai_tokenizers/TensorFlow2/two_spm/1`

## Results and limitations

CRISPR AI is the portfolio project label. The code models sequence/mutation text; it is not a verified guide-RNA designer, genome editor, therapeutic system, or biological validation. Related protein translation notebooks are supporting experiments, not evidence of a working integrated pipeline. Tokenizer/model files and source datasets must be supplied separately.

The recovered Kaggle source exports contain no retained executed outputs; this repository therefore does not advertise a numeric result based on notebook titles or training settings. Training was not rerun as part of organization. Structural validation is not a runtime or scientific validation.

## Attribution and rights

Original notebook attribution, comments, and tutorial links are preserved. Standard TensorFlow/Keras examples and tutorial-style code should not be represented as newly invented algorithms. The precise human/AI/tool contribution history is not reconstructed by this archive. No blanket new license is assigned to third-party material. Datasets, pretrained models, and tutorial-derived content retain their own licenses and access requirements; their bytes are not bundled here.

The attention/encoder-decoder organization includes TensorFlow tutorial-style components; see the [TensorFlow Transformer tutorial](https://www.tensorflow.org/text/tutorials/transformer) for the standard architecture pattern. This is an attribution reference, not a verified line-by-line authorship audit.
