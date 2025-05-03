## 🎯 Precision vs. Recall – Clear Understanding

Imagine you're building a **spam email detector**.

* **Goal:** Predict whether an email is **spam** or **not spam**.

There are 4 possible outcomes in any classification problem:

|                      | Predicted: Spam       | Predicted: Not Spam   |
| -------------------- | --------------------- | --------------------- |
| **Actual: Spam**     | ✅ True Positive (TP)  | ❌ False Negative (FN) |
| **Actual: Not Spam** | ❌ False Positive (FP) | ✅ True Negative (TN)  |

---

### 🔎 What is **Precision**?

> **Precision** = How many predicted *spams* were actually spam?

**Formula:**

```
Precision = TP / (TP + FP)
```

### 📌 Example:

* Model predicted 100 emails as spam.
* 80 were actually spam → True Positives (TP)
* 20 were wrongly predicted as spam → False Positives (FP)

```
Precision = 80 / (80 + 20) = 0.80 or 80%
```

#### ✅ Interpretation:

> Out of all emails your model called **spam**, 80% were correct.
> **High precision = few false alarms.**

---

### 🔁 What is **Recall**?

> **Recall** = How many of the actual spams did the model catch?

**Formula:**

```
Recall = TP / (TP + FN)
```

### 📌 Example:

* There were 120 spam emails in total.
* Model caught 80 of them → TP
* Missed 40 of them → FN

```
Recall = 80 / (80 + 40) = 0.666 or 66.6%
```

#### ✅ Interpretation:

> Out of all real spam emails, your model caught 66.6%.
> **High recall = fewer missed actual cases.**

---

## 🎯 Summary Table:

| Metric    | Focuses On                                 | Good When You Want...                                   |
| --------- | ------------------------------------------ | ------------------------------------------------------- |
| Precision | Being **accurate** in positive predictions | Avoid false alarms (e.g., important emails marked spam) |
| Recall    | **Catching all** actual positives          | Catch all true cases (e.g., no spam escapes detection)  |

---

## 🤔 Final Tip for Students:

> Think of **Precision** as “**How precise is your aim?**”
> Think of **Recall** as “**How much did you remember to catch?**”

---

Would you like me to create a visual example in Python (confusion matrix, precision-recall curve) to show live during your webinar?
