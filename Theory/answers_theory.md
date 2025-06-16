# Theoretical Section – Part 1: Understanding AI Tools

---

## Q1: Explain the primary differences between TensorFlow and PyTorch. When would you choose one over the other?

| Feature              | TensorFlow                                           | PyTorch                                                |
|----------------------|------------------------------------------------------|---------------------------------------------------------|
| Origin               | Createded by Google                                  | Created by Meta                            |
| Computation Graph    | Static graph (TF 1.x), dynamic graph in TF 2.x       | Dynamic computation graph (eager execution)             |
| Ease of Debugging    | More complex in earlier versions; improved in TF 2.x | Easier to debug due to Python-native design             |
| Deployment Tools     | TensorFlow Lite, TensorFlow.js, TensorFlow Serving   | TorchScript, ONNX, limited web/mobile support           |
| Community & Support  | Strong in production; Google ecosystem               | Popular in research; very active research community     | 
| Syntax               | Stronger but more verbose                            | Python-based and perceptive             |                                                       |

**When to Choose:**

- Use **TensorFlow** for:
  - Production-grade deployment
  - Web/mobile integration (TFLite, TF.js)
  - Access to tools like TensorBoard, TFX, and TPU acceleration

- Use **PyTorch** for:
  - Research and academic prototyping
  - Dynamic model architectures (e.g., RNNs, transformers)
  - Fast debugging using native Python tools

---

## Q2: Describe two use cases for Jupyter Notebooks in AI development.

1. **Model Prototyping and Experimentation**
   - Jupyter Notebooks allow step-by-step development.
   - Data scientists can test models, visualize results (e.g., loss curves), and modify parameters interactively.

2. **Educational and Collaborative Demos**
   - Ideal for tutorials, teaching, and reproducible research.
   - Allows integration of markdown, LaTeX, images, and executable code all in one place.

---

## Q3: How does spaCy enhance NLP tasks compared to basic Python string operations?

| Feature                   | spaCy                                           | Python String Methods            |
|---------------------------|--------------------------------------------------|----------------------------------|
| Language Model            | Pretrained NLP pipelines with linguistic rules   | No language understanding        |
| Tokenization              | Rule-based and language-aware                    | Basic `split()`, limited context |
| Named Entity Recognition  | Built-in, pretrained                            | Not available                    |
| POS Tagging               | Yes                                              | Not available                    |
| Lemmatization             | Yes                                              | Not available                    |
| Dependency Parsing        | Yes                                              | Not supported                    |
| Performance               | Fast (Cython-optimized)                          | Slower on large text corpora     |

**Summary:**
While Python string functions are useful for simple tasks like substring matching or splitting text, **spaCy** offers robust natural language understanding features like entity recognition, POS tagging, and parsing, making it ideal for real-world NLP applications.

---
