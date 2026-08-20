# Sign Language Question Answering: A New Task, Benchmark, and Baseline for Sign Language Understanding

[![arXiv](https://img.shields.io/badge/arXiv-2607.27826-b31b1b.svg)](https://arxiv.org/abs/2607.27826)
[![Dataset](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-SignQA--2026-yellow)](https://huggingface.co/datasets/hulala/SignQA-2026)

This repository accompanies the paper **“Sign Language Question Answering: A
New Task, Benchmark, and Baseline for Sign Language Understanding.”**

We introduce **Sign Language Question Answering (SLQA)**, a task that evaluates
sign language understanding by asking models to answer natural-language
questions grounded in sign videos. Unlike recognition and translation tasks
with fixed outputs, SLQA evaluates whether a model can retrieve and reason about
different aspects of the same video.

## SignQA-2026

We construct two multilingual benchmarks from the annotations of CSL-Daily and
PHOENIX-2014T. The current Hugging Face release contains question-answer
annotations only; source videos are not redistributed.

| Configuration | Language | Train | Validation | Test | Total |
| --- | --- | ---: | ---: | ---: | ---: |
| `csl-daily-qa` | Chinese | 92,000 | 5,385 | 5,880 | 103,265 |
| `phoenix14t-qa` | German | 35,480 | 2,595 | 3,210 | 41,285 |
| **Total** | — | **127,480** | **7,980** | **9,090** | **144,550** |

The benchmark contains 28,910 unique video IDs and covers five complementary
question categories:

- M1: Position Reasoning
- M2: Structural Reasoning
- M3: Visual Search
- M4: Gloss Recognition
- M5: Translation Understanding

Download and preview the annotations on
[Hugging Face](https://huggingface.co/datasets/hulala/SignQA-2026).
To use video inputs, please obtain CSL-Daily and PHOENIX-2014T separately and
follow their original access and license terms.

## TODO

- [x] Release the paper
- [x] Release the SignQA-2026 annotations
- [ ] Release training and evaluation code
- [ ] Release pretrained checkpoints

## Citation

If you find this work useful, please cite:

```bibtex
@misc{gan2026signlanguagequestionanswering,
  title         = {Sign Language Question Answering: A New Task, Benchmark,
                   and Baseline for Sign Language Understanding},
  author        = {Shiwei Gan and Lichen Wang and Xiao Liu and Yafeng Yin and
                   Kuizhuang Liu and Sanglu Lu and Lei Xie},
  year          = {2026},
  eprint        = {2607.27826},
  archivePrefix = {arXiv},
  primaryClass  = {cs.AI},
  doi           = {10.48550/arXiv.2607.27826},
  url           = {https://arxiv.org/abs/2607.27826}
}
```

