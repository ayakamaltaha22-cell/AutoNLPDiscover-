# AutoNLP-Discover

AutoNLP-Discover is a modular AI-driven framework that automates the entire NLP research lifecycle — from research gap identification to model generation, experiment optimization, and scientific insight generation. It integrates reinforcement learning, neural architecture search, information extraction, and large language models to accelerate and enhance NLP research workflows.

---

## 🔍 Key Features

- **Research Gap Identifier**: Uses knowledge graphs and contrastive citation analysis to discover underexplored NLP tasks.
- **RL-Based Neural Architecture Search (RL-NAS)**: Automatically generates novel model architectures based on task needs.
- **RL Experiment Executor**: Optimizes hyperparameters and training settings in a closed-loop, reinforcement-based setup.
- **LLM-Based Insight Generator**: Auto-generates summaries, abstracts, and visualizations using GPT-style models.

---

## 🧱 Project Structure

```bash
AutoNLP-Discover/
├── main.py                         # Orchestrates full pipeline
├── extraction/
│   ├── preprocess.py               # PDF/HTML text extraction
│   ├── ner.py                      # Named Entity Recognition
│   └── relation_extraction.py     # Relation extraction using BERT
├── graph/
│   └── build_graph.py             # Builds NLP Knowledge Graph (Neo4j)
├── gap_identifier/
│   └── rgim.py                    # Research gap detection logic
├── model_generator/
│   └── rl_nas.py                  # RL-based neural architecture search
├── experiment_executor/
│   └── rlexecutor.py             # RL agent for tuning experiments
├── insight_generator/
│   ├── summarizer.py             # GPT-based result summarization
│   └── visualizer.py             # Performance visualization with matplotlib
```

---

## ⚙️ Installation

1. Clone this repo:
```bash
git clone https://github.com/your-username/AutoNLP-Discover.git
cd AutoNLP-Discover
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. (Optional) Set up Neo4j for knowledge graph storage:
- Install Neo4j Community Edition
- Set password in `graph/build_graph.py`

---

## 🚀 How to Run

Run the entire NLP automation pipeline:

```bash
python main.py
```

---

## 📊 Example Output

- Knowledge Graph in Neo4j browser
- Auto-generated models and their performance scores
- Visual summaries: accuracy/loss plots, confusion matrices
- GPT-generated research abstracts and summaries

---

## 📘 Requirements

- Python ≥ 3.8
- Neo4j (for graph storage)
- PyTorch
- Transformers (HuggingFace)
- Matplotlib
- scikit-learn
- spaCy, Tabula-py, GROBID (optional for advanced IE)

---

## 🧠 Citation

If you use this framework, please cite the original paper:

> Taha, K. (2025). AutoNLP-Discover: A Reinforcement and Knowledge-Guided Framework for Accelerating NLP Research.

---

## 📬 Contact

For questions, contact:  
**Dr. Kamal Taha**  
Associate Professor, Khalifa University, UAE  
Email: [your-email@example.com]
