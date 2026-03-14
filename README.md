# 🏺 Multi-Modal Artifact Valuation System

A robust, production-ready machine learning pipeline for estimating preservation scores of artifacts, integrating both structured metadata and natural language descriptions.

---

## 📚 Overview

This project implements a modular, end-to-end ML workflow with:

- Data ingestion, validation & transformation (text + structured)
- Advanced feature engineering (TF-IDF, count vectorizer, and transformer-based text embeddings)
- Model training/comparison across tree-based, linear, and neural regressors
- Scalable experiment tracking & artifact management via MLflow and DagsHub
- Stage-wise orchestration with thorough logging, error handling, and checkpointing

---

## ⚙️ Project Structure
```
├── .github/
│   └── workflows/
├── artifacts/
│   ├── data_ingestion/
│   ├── data_preprocessed/
│   ├── data_transformation/
│   ├── data_validation/
│   ├── model_evaluation/
│   └── model_trainer/
├── catboost_info/
│   ├── learn/
│   └── tmp/
├── config/
├── data/
│   └── Images/
├── logs/
├── research/
│   └── models/
└── src/
    ├── components/
    ├── config/
    ├── constants/
    ├── entity/
    ├── logging/
    ├── pipeline/
    └── utils/
```


---


## 🏗️ Features

- **Multi-modal:** Combines structured and unstructured text info for greater predictive power.
- **Flexible feature engineering:** Modular, supports TF-IDF, CountVectorizer, and transformer embeddings (MiniLM, mpnet, distilBERT).
- **Model-agnostic benchmarking:** Trains XGBoost, LightGBM, CatBoost, Ridge, SVR, MLP, RandomForest, and more.
- **Full MLOps integration:** Automatic logging of params, metrics, and artifacts to MLflow and DagsHub.
- **Easy stage resuming:** Each pipeline stage can be run/tested/debugged independently.
- **Clear checkpointing/logging:** All major operations logged, errors handled gracefully.


---

## 📄 Documentation & Customization

- Pipeline configuration: `config.yaml`
- MLflow tracking: Set via `mlops_config` in config
- Skip stages / resume: Use flag files or invoke `src.pipeline` modules directly
- Feature engineering: All transformers and preprocessor files saved under `artifacts/`

---

## 🤝 Contributing

Contributions welcome!  
Open issues or PRs for improvements, new model/feature support, or integrating more MLOps tools.

---

## 📄 License

[MIT](LICENSE) © 2025 

---

## 📫 Contact

For help or collaboration, open a GitHub issue or contact: bhavyachillara413@gmail.com

---

## 🙏 Acknowledgements

- [MLflow](https://mlflow.org/)
- [DagsHub](https://dagshub.com/)
- [scikit-learn](https://scikit-learn.org/)
- [HuggingFace Transformers](https://huggingface.co/)



