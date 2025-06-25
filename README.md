# 🧠 Bag of Words (BoW) Text Vectorization from Scratch

This repository contains a Python script that implements the **Bag of Words (BoW)** technique **from scratch**, without using external libraries like `scikit-learn`. It's intended for **beginners in Machine Learning** and **Natural Language Processing (NLP)** who want to understand how text data can be converted into numerical vectors.

---

## 📄 What is Bag of Words?

The Bag of Words model is a technique used to convert **text into numerical features** for use in machine learning models. It:

* Builds a **vocabulary** of unique words.
* Converts each sentence into a **vector** based on **word frequency**.

For example, with:

```
"I love machine learning"
"I love coding"
```

You get a vocabulary like:

```
['coding', 'learning', 'love', 'machine', 'i']
```

Then each sentence becomes a vector of word counts:

```
[0, 1, 1, 1, 1]  → for "I love machine learning"
[1, 0, 1, 0, 1]  → for "I love coding"
```

---

## 📁 File Structure

```
├── bow.py             # Main Python script that reads a text file and creates BoW vectors
├── test.txt           # Text file with input sentences (one per line)
└── README.md          # Project explanation (you are here!)
```

---

## 🚀 How to Use

### 1. 📥 Clone the Repository

```bash
git clone https://github.com/yourusername/bag-of-words-from-scratch.git
cd bag-of-words-from-scratch
```

### 2. 📝 Prepare the Input File

Create a file called `test.txt` in the same directory. Each line should be a sentence:

```
I love machine learning
I love coding
Machine learning is fun
```

### 3. ▶️ Run the Script

```bash
python bow.py
```

You will see the following printed:

* The list of original documents.
* The tokenized version (split words).
* The vocabulary (unique sorted words).
* The mapping of words to indices.
* The Bag of Words vectors for each sentence.

---

## 🔍 Code Overview

Here's what the script does step-by-step:

1. **Read File**: Reads lines from `test.txt`.
2. **Tokenize**: Converts each line to lowercase and splits into words.
3. **Build Vocabulary**: Creates a sorted list of unique words.
4. **Map Words to Indices**: Uses a dictionary for fast lookup.
5. **Generate Vectors**: Creates a frequency vector for each sentence.
6. **Print Results**: Displays all the above.

All of this is done **without using external libraries**, which helps you understand the underlying logic clearly.

---

## 📚 For Beginners

If you're learning:

* Start by modifying `test.txt` with your own sentences.
* Try adding punctuation removal or using binary BoW (0/1 instead of counts).
* Wrap the logic in functions for reuse.

---

## 🧼 To Do (Improvements You Can Try)

* [ ] Add punctuation removal
* [ ] Convert to binary BoW (presence/absence)
* [ ] Export vectors to a CSV file
* [ ] Turn into a reusable function or class
* [ ] Add a command-line interface

---

## 🤝 Contributing

Contributions, suggestions, and questions are welcome! Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License. Feel free to use, modify, and share.

---

Would you like this README saved as a `README.md` file, or want me to help you improve the script further (e.g. punctuation cleaning, CSV export)?
