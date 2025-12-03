# 📊 Slice Evaluation Summary — Post LLM-Generated Examples

This summary highlights the performance of the `roberta` model across various tweet slices after augmenting the dataset with LLM-generated examples. The evaluation was conducted using Zeno’s slicing interface, with accuracy as the primary metric.

## 🔍 Accuracy Overview

| Slice Name                  | Accuracy | Instances |
|----------------------------|----------|-----------|
| All instances              | 0.70     | 510       |
| Positive Label             | 1.00     | 4         |
| Negative Tweet             | 0.60     | 20        |
| Long Tweets                | —        | 0         |
| Low Confidence Predictions | —        | 0         |
| Ambiguous Tweets           | 0.70     | 495       |
| Emoji Tweet                | 1.00     | 2         |
| Emoji Tweets               | 1.00     | 1         |
| Slang Tweets               | 0.71     | 17        |
| Question Tweets            | 0.66     | 58        |

## 🧠 Insights

- **Positive Label Tweets** showed perfect accuracy, though the sample size was small.
- **Negative Tweets** and **Question Tweets** revealed weaknesses in sarcasm and rhetorical tone.
- **Ambiguous Tweets** had moderate accuracy, suggesting the model defaults to neutral when uncertain.
- **Emoji Tweets** performed well, but the low instance count limits generalization.
- **Slang Tweets** were handled reasonably, though cultural nuance remains a challenge.

## 📸 Screenshots

- `lab4_accuracy_table.png` → Zeno interface showing slice-level accuracy.
- `slice_evaluation_table.png` → Markdown table summarizing rationale, observed behavior, and implications.

These results support the need for more diverse and nuanced test cases, especially in sarcasm, ambiguity, and informal language.

