The Fake News Detective Story

Imagine you’re the editor of a huge newspaper. Every day, thousands of articles land on your desk — some are *real news*, some are *fake stories*. You don’t have the time to read each one carefully, so you hire a *digital detective*.

Here’s how your detective works:

1. Reading the articles
   First, the detective looks at all the news pieces. But instead of getting distracted by small talk words like *“the, is, was”, it focuses on the meaningful words. Importantly, it pays close attention to *negations* like “not” — because “not true”* is very different from “true”.

2. Turning words into numbers
   The detective doesn’t really understand words like we do. So it creates its own secret dictionary: every word becomes a unique number. For example, *president → 45*, *election → 112*, *scandal → 980*.
   Now every article is just a sequence of numbers.

3. Making stories the same length
   Some articles are long, some short. The detective likes order — so it chops or stretches each article to the same length (say, 500 words). Like putting them all into *equal-sized boxes*.

4. Learning the patterns
   Now comes the fun part. The detective has a *memory (LSTM)*. It reads through each article word by word and tries to understand the flow of the story. For example:

   * Real news might use phrases like *“official sources confirmed”*.
   * Fake news might use *“shocking truth they don’t want you to know”*.
     Over time, it learns these subtle patterns.

5. Making the judgment
   When a new article arrives, the detective scans it and finally whispers:

   * “This looks **real**” (label = 1), or
   * “This smells **fake**” (label = 0).

6. **Improving over time**
   Just like any detective, it gets better the more cases it handles. If it makes a mistake, we correct it — and it updates its thinking.

In simple words:
This algorithm is like a **digital detective trained on thousands of articles**. Instead of reading with human intuition, it uses math to spot patterns in words and sentences, and then decides whether a news story is likely **fake or real**.

---

This project uses an LSTM-based deep learning model to classify news as **real or fake**, using text preprocessing and neural network modeling in Keras.

## 📌 Project Highlights
- Text tokenization & padding
- LSTM-based sequential model
- Model evaluation: Accuracy, Confusion Matrix


## 🧪 Technologies Used
- Python
- TensorFlow / Keras
- Scikit-learn
- Matplotlib / Seaborn

📈 Results
Model shows strong performance on validation set and interprets patterns using  confusion matrix.

---

### ✅ `requirements.txt`
```txt
tensorflow
scikit-learn
matplotlib
numpy
pandas
seaborn
