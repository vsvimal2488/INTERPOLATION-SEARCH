# Interpolation Search vs Binary Search Performance Analysis

This Python program implements and benchmarks two fundamental searching algorithms: **Interpolation Search** and **Binary Search**. It compares their performance across various dataset sizes, measuring both execution time and the number of comparisons required to find a target value in a sorted array.

## 📋 Features

- **Interpolation Search Implementation:** An optimized search algorithm that uses the value of the target to estimate its position (probe) within the array.
- **Binary Search Implementation:** A classic divide-and-conquer search algorithm for comparison.
- **Performance Benchmarking:** Automatically tests both algorithms on random sorted datasets of increasing sizes (10,000 to 1,000,000 elements).
- **Metrics:** Measures and displays:
  - Execution time (in milliseconds)
  - Number of comparisons made during the search
- **Example Execution:** Includes a hardcoded demo run to visually verify the algorithm's correctness.

## 🧠 How the Algorithms Work

### Interpolation Search
- **Time Complexity:** `O(log log n)` on average, `O(n)` in the worst case.
- **Space Complexity:** `O(1)`.
- **Logic:** Instead of always checking the middle element like Binary Search, it calculates a *probe* position using a linear interpolation formula. It works exceptionally well on uniformly distributed sorted data.

### Binary Search
- **Time Complexity:** `O(log n)`.
- **Space Complexity:** `O(1)`.
- **Logic:** It repeatedly divides the search interval in half, discarding the half that cannot contain the target value.

## 🛠️ Requirements

- **Python 3.x** (The code uses `time.perf_counter()` which is available in Python 3.3+).
- No external libraries are required (uses built-in `time`, `random`, and `sys` modules).

## 🚀 How to Run

1. Save the Python code as `interpolation_search.py`.
2. Open your terminal or command prompt.
3. Navigate to the folder containing the file.
4. Run the following command:

```bash
python interpolation_search.py
