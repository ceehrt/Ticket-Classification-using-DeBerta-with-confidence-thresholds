# Ticket Classification Using DeBERTa with Confidence Thresholds

This project applies **DeBERTa** for automatic ticket classification and analyses predictions using different confidence thresholds.

The objective is to identify high-confidence predictions and uncertain predictions that may require further verification.

## Confidence Thresholds

The model is evaluated using five confidence thresholds:

* 50%
* 60%
* 70%
* 80%
* 90%

For each ticket, DeBERTa predicts a ticket category and generates a confidence score. Predictions below the selected threshold can be identified for further review.

```python id="q7r3mx"
thresholds = [0.50, 0.60, 0.70, 0.80, 0.90]
```

## Workflow

```text id="hn8t2c"
Ticket Data
    ↓
Data Preprocessing
    ↓
DeBERTa Classification
    ↓
Prediction + Confidence Score
    ↓
Confidence Threshold

```

## Technologies

* Python
* Google Colab
* PyTorch
* Hugging Face Transformers
* DeBERTa
* Scikit-learn
* Pandas

## Environment

| Component    | Version               |
| ------------ | --------------------- |
| PyTorch      | 2.11.0+cu128          |
| Transformers | 4.54.0                |
| Datasets     | 4.0.0                 |
| Scikit-learn | 1.6.1                 |
| Pandas       | 2.2.3                 |
| CUDA         | 12.8                  |
| GPU          | NVIDIA A100-SXM4-80GB |

## Evaluation

The project evaluates DeBERTa using standard classification metrics and compares predictions across different confidence thresholds.

The threshold analysis helps examine the trade-off between the **number of predictions accepted** and the **confidence of those predictions**.

## Future Work

This project can be extended by adding:

* Verification of low-confidence predictions
* Explainable AI (XAI)
* LLM-based verification
* Agentic AI workflow for automated ticket handling

## Author

**Orapin Pakkarapanit**

Research interests: **Artificial Intelligence, NLP, Transformer Models, Explainable AI, and Agentic AI**
