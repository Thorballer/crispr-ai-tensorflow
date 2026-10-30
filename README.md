# CRISPR AI — TensorFlow research prototype

A sequence-to-sequence research prototype conditioning on sequence data and effect descriptions to predict mutation-change tokens, with related protein/text experiments.

## Notebooks

- [science-fair-gene-mutation.ipynb](notebooks/science-fair-gene-mutation.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-gene-mutation)
- [tokenizer-dna-mutations.ipynb](notebooks/tokenizer-dna-mutations.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/tokenizer-dna-mutations)
- [gene-dataset.ipynb](notebooks/gene-dataset.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/gene-dataset)
- [science-fair-function-to-protein.ipynb](notebooks/science-fair-function-to-protein.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-function-to-protein)
- [science-fair-protein-to-process.ipynb](notebooks/science-fair-protein-to-process.ipynb) — [original Kaggle notebook](https://www.kaggle.com/code/thorballer/science-fair-protein-to-process)

Start with `science-fair-gene-mutation`; the other notebooks cover tokenization, data preparation, and related protein/text experiments. “CRISPR AI” is the project name: this models mutation tokens, not a biologically validated genome-editing system.

## Running

Open the original Kaggle notebook, attach its referenced data/models, choose the hardware expected by its setup cells, and run cells in order. Review install, login, and file-writing cells first.

For local use, install `requirements.txt` and adapt `/kaggle/input` paths. Dependencies are inferred from imports, not a tested lockfile; older APIs may need adjustment.

### Referenced Kaggle datasets

- [thorballer/all-uniprot-isodata](https://www.kaggle.com/datasets/thorballer/all-uniprot-isodata)
- [thorballer/full-unlinked-mutations-ds](https://www.kaggle.com/datasets/thorballer/full-unlinked-mutations-ds)
- [thorballer/human-protein-dataset](https://www.kaggle.com/datasets/thorballer/human-protein-dataset)
- [thorballer/parsed-dna-mutations](https://www.kaggle.com/datasets/thorballer/parsed-dna-mutations)

### Referenced Kaggle models/tokenizers

- `thorballer/dna-mutations-tokenizers/TensorFlow2/default/4`
- `thorballer/protein_ai_tokenizers/TensorFlow2/default/1`
- `thorballer/protein_ai_tokenizers/TensorFlow2/two_spm/1`

## Status and source

These exports have no saved execution outputs. Training was not rerun, so this archive reports no benchmark scores.

Daniel Goldberg's Kaggle notebooks are preserved with source links and hashes in [PROVENANCE.json](PROVENANCE.json). Documentation was added for this archive.

Original comments, credits, and tutorial links are retained. Datasets and dependencies have their own licenses; no new blanket license is assigned. Architecture reference: [TensorFlow Transformer tutorial](https://www.tensorflow.org/text/tutorials/transformer).
