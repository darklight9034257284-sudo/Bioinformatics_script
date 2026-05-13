# HMM-project

This is a small, simple HMM example I wrote to try out basic ideas from class. It models a short DNA sequence using five states:

- `s` (start)
- `E` (exon)
- `5` (a second exon-style state used in the toy model)
- `I` (intron)
- `e` (end)

The script `hmm.py` computes the log-probability of a few candidate state paths for a hard-coded DNA sequence and prints the most likely one. It's meant as a learning exercise — not a production tool.

## Requirements

- Python 3
- `numpy`

I used a virtualenv to keep things clean. Example setup:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install numpy
```

## How to run

From the repo root:

```bash
python HMM-project/hmm.py
```

Or from inside the `HMM-project` folder:

```bash
cd HMM-project
python hmm.py
```

The script will print each candidate path and its log-probability, then print which path had the highest log-probability.

## Inputs and outputs

- Input: the sequence is currently hard-coded in `hmm.py` as `query_sequence`.
- Output: printed log-probabilities for each candidate path and the best-scoring path.

