# Advanced Learning for Text and Graph Data (ALTEGRAD)
**Master MVA (Mathématiques, Vision, Apprentissage) — ENS Paris-Saclay**

Welcome to the repository for **ALTEGRAD**, a core course offered in the renowned M2 MVA research master's program at **ENS Paris-Saclay** (co-accredited with the Institut Polytechnique de Paris and shared with Université Paris Cité). 

* **Course Instructor:** Prof. Michalis Vazirgiannis
* **Teaching Assistants:** Amr Mohamed, Yang Zhang
* **Official Course Page:** [Master MVA ALTEGRAD Course Hub](https://www.master-mva.com/cours/cat-advanced-learning-for-text-and-graph-data-altegrad/)

---

## 💡 What is ALTEGRAD?

**ALTEGRAD** (*Advanced Learning for Text and Graph Data*) is an advanced machine learning and artificial intelligence course focused on processing, modeling, and generating data structured as **sequences/text** and **graphs**. 

The curriculum bridges cutting-edge foundational theory with heavy-duty practical implementations, covering fields that dictate modern AI research and industrial deployment:

1. **Natural Language Processing (NLP) & Large Language Models (LLMs):**
   * Attention mechanisms, Transformer architectures, and context scaling.
   * Parameter-Efficient Fine-Tuning (PEFT/LoRA), model quantization (`bitsandbytes`), and instruction tuning.
   * Efficient evaluation frameworks and sovereign/multilingual LLM adaptation.

2. **Deep Learning for Graphs (DLG):**
   * Graph representation learning and core-decomposition metrics ($k$-core, graph degeneracy) applied to text mining and network analysis.
   * Geometric and equivariant deep learning ($SE(3)/E(3)$ invariant GNNs) for physical, chemical, and relational systems.
   * Graph-augmented LLMs, linking reasoning pipelines with structured knowledge bases and relational databases.

---

## 🚀 Lab Session 2 Overview: Pretraining & Supervised Finetuning

The goal of Lab Session 2 is to gain hands-on experience in adapting Large Language Models (LLMs) to specific tasks using parameter-efficient fine-tuning (PEFT), quantization, and prompt formatting techniques:

* **Instruction Fine-Tuning:** Adapting a pretrained base model into a helpful conversational assistant using instruction-response pairs.
* **Model Architecture & Quantization:** Loading `Qwen/Qwen3.5-0.8B-Base` using 4-bit NormalFloat (NF4) quantization via `bitsandbytes` to minimize GPU VRAM consumption on consumer-grade hardware (such as a Google Colab T4 GPU).
* **Parameter-Efficient Fine-Tuning (LoRA):** Injecting low-rank adaptation matrices into the token-mixing layers and MLP blocks to train only a small fraction of total parameters (~21.6M trainable parameters out of ~0.75B).
* **French Summarization Task:** Fine-tuning the model on `giuliadc/orangesum_5k` (a French news summarization dataset) with custom chat templates and completion-only loss masking.
* **Evaluation & Tool Calling:** Comparing generations and held-out evaluation loss before and after fine-tuning, followed by functional tool-calling setups.

---

## 🛠️ Requirements & Installation

This lab is designed to run in environments like **Google Colab (T4 GPU)** or local machines with CUDA support:

```bash
pip install -q "transformers==5.18.0" "accelerate==1.15.0" "peft==0.21.2" "bitsandbytes==0.50.2"
pip uninstall -y -q torchao
```

---

## 📂 Repository Structure

```text
├── labs/
│   ├── lab-01-nlp-attention/         # Transformers & Self-Attention mechanics
│   └── lab-02-peft-finetuning/       # QLoRA, Quantization, and Instruction Tuning
├── challenge/                        # End-of-course data challenge code and submissions
└── README.md
```

---

## 🔗 Quick Links & Resources

* **Master MVA Website:** [master-mva.com](https://www.master-mva.com/)
* **ALTEGRAD Syllabus & Content:** [Course Page on Master MVA](https://www.master-mva.com/cours/cat-advanced-learning-for-text-and-graph-data-altegrad/)
* **ENS Paris-Saclay:** [ens-paris-saclay.fr](https://ens-paris-saclay.fr/)