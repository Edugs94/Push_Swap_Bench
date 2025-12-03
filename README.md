# 📊 Push Swap Benchmark

A lightweight, dynamic **Bash script** designed to stress-test, validate, and measure the efficiency of your **Push Swap** project (42 School curriculum).

<img src="https://github.com/user-attachments/assets/37c5dd2b-fa6d-409f-8171-d1fcdf284bf9" alt="bench_working" width="400">

---

## 🚀 Features

* **Dynamic Range:** Automatically adjusts the pool of random numbers based on the requested stack size (e.g., Stack 100 uses range -200 to 200; Stack 500 uses -1000 to 1000).
* **Safety Limits:** Includes a hard limit (Max 1000 numbers) to prevent system freezes or memory overflows during testing.
* **Statistical Average:** Runs **50 iterations** per execution and calculates the precise average move count.
* **Zero Dependencies:** Runs natively in Bash (uses `seq`, `shuf`, `tr`, `wc`). No Python, Ruby, or external libraries required.

---

## 🛠️ Installation

1.  **Clone this repository** or download the `bench.sh` file.
2.  Move the `bench.sh` script into the **root directory** of your Push Swap project (where your `push_swap` executable is located).

```bash
cp /path/to/bench.sh /path/to/your_push_swap_project/
```
Grant execution permissions:
```bash
chmod +x bench.sh
```
## 💻 Usage

Ensure your **./push_swap** executable is compiled and ready. Then, run the script specifying the number of elements you want to test.

---

### Standard Test (100 Numbers)

<pre><code>sh bench.sh 100</code></pre>
### Stress Test (500 Numbers)

<pre><code>sh bench.sh 500</code></pre>
