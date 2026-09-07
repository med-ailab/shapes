> **Med AI Lab · Innopolis University**  
> Code and data released alongside a peer-reviewed publication.  
> Original repository by [Danis Alukaev](https://github.com/DanisAlukaev): <https://github.com/DanisAlukaev/shapes>

---

Synthetic dataset of primitive shapes with generated textual descriptions, used to evaluate cross-modal concept bottleneck models.

### Paper

- **Cross-Modal Conceptualization in Bottleneck Models**  
  D. Alukaev, S. Kiselev, I. Pershin, B. Ibragimov, V. Ivanov, A. Kornaev, I. Titov  
  *EMNLP 2023, main track* · [link](https://aclanthology.org/2023.emnlp-main.318/)

### About the lab

The **Med AI Lab** at Innopolis University works on medical AI in which the clinician is part
of the system rather than its user: eye tracking of radiologists, gaze as a supervision signal
for medical imaging, electronic health records, and the modelling of human attention in
language models.

[Website](https://ilya-pershin.com/lab/) · [Publications](https://ilya-pershin.com/publications/) · [All code](https://github.com/med-ailab) · i.pershin@innopolis.ru

### License

The original repository does not carry a licence file, so no reuse rights are granted
by default. Before reusing this code, contact the author or the lab.

---

*Everything below is the original README from [DanisAlukaev/shapes](https://github.com/DanisAlukaev/shapes), left unchanged.*

---
<div align="center" height="130px">
  <img src="./docs/images/logotype.png" alt="Logotype"/><br/>
  <p></p>
</div>

> Primitive shapes to check how interpretable your latent representations are! 

## 🎯 Motivation

While quantifying interpretability of machine learning algorithm, we often need to compare the predicted latent representation with underlying factors of generative process. Thus, introducing a simple dataset that does not require domain knowledge yet possess ground truth attributes annotation might be beneficial for a hypotheses testing. 

![sample](./docs/images/sample.png)

For this reason and primarily for benchmarking we propose a synthetic dataset of primitive shapes. The image is a white canvas with random shape (i.e., square, triangle, circle) of random color (i.e., red, green, blue), and random size (i.e., small, medium, large). Caption is generated from visual parameters of a shape, its location, and words sampled from the vocabulary, using a hand-written grammar. The vector of attributes encodes shape and color, their combination represents a target class y.

## 📖 Citation

This dataset as a part of a research paper ["Cross-Modal Conceptualization in Bottleneck Models"](https://arxiv.org/abs/2310.14805) was introduced in EMNLP 2023. To cite it please use the following bibtex:
```bibtex
@inproceedings{
    alukaev2023crossmodal,
    title={Cross-Modal Conceptualization in Bottleneck Models},
    author={Danis Alukaev and Semen Kiselev and Ilya Pershin and Bulat Ibragimov and Vladimir V. Ivanov and Alexey Kornaev and Ivan Titov},
    booktitle={The 2023 Conference on Empirical Methods in Natural Language Processing},
    year={2023},
    url={https://openreview.net/forum?id=ghF1EB6APx}
}
```