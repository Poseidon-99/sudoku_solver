# 🧠 Sudoku Solver using Deep Learning (Built from Scratch)

This project explores how neural networks can be trained to **learn logical reasoning**—specifically through the challenge of solving 9x9 Sudoku puzzles. Unlike traditional rule-based solvers, this solution uses a **custom-designed deep convolutional neural network** that learns to fill in missing numbers by recognizing patterns across rows, columns, and 3x3 boxes.

---

## 🔍 Project Highlights

- 🧩 Built a **9-layer deep CNN** designed to mimic human logical solving strategies
- 📊 Trained on a large dataset of Sudoku puzzles + solutions
- 🧠 Model takes multi-channel input representing rows, columns, and boxes
- 🎯 Learns to predict **only the empty cells** (not the clues)
- 🔄 Evaluated performance using masked prediction accuracy and solution validity
- ✅ Developed fully from scratch — **no prebuilt solvers or libraries used**

---

## 💡 Why This Project?

Sudoku is a constrained, logic-based problem — a perfect testbed for training models to **infer structure, patterns, and rules**. This project is not just about solving a game — it's about teaching a neural network to reason in a structured space.

> “What if we could train deep learning models to learn reasoning like a human solver?”

---

## 🛠️ Architecture Overview

- **Input**: 9×9 Sudoku board, converted into:
  - Box matrix
  - Row matrix
  - Column matrix
- **Model**:
  - Deep CNN with 9 layers, following a bottleneck-style architecture
  - Hidden layers extract spatial and logical features
  - Final layer reshapes output back to a 9x9 grid of predicted digits (1–9)
- **Loss Function**: Categorical Crossentropy on only the empty cells
- **Evaluation**:
  - Accuracy on masked positions (empty cells)
  - Puzzle completion rate (100% valid solution)

---

## 🧪 Sample Output

| Input Puzzle | Predicted Solution |
|--------------|--------------------|
| ![input](images/sample_input.png) | ![output](images/sample_output.png) |

---

## 📁 Project Structure

