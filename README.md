# 🚀 FireDucks vs Pandas: Speeding Up AI/ML Pipelines

A quick benchmark comparing **FireDucks** with **Pandas** for common data tasks in machine learning workflows — like reading, filtering, grouping, and sorting large datasets.

---

## ⚡ Why FireDucks?

Pandas is great, but it struggles with big data. **FireDucks** is a drop-in replacement built for performance:

* Faster execution (especially on large datasets)
* Lazy evaluation for better optimization
* Lower memory usage
* Same Pandas-like syntax

---

## 🧪 Benchmark Summary

| Operation       | Pandas (ms) | FireDucks (ms) |
| --------------- | ----------- | -------------- |
| Read CSV        | 344.89      | 35.67          |
| Filter Rows     | 17.69       | 17.82          |
| GroupBy Avg     | 59.76       | 13.19          |
| Sort Descending | 0.87        | 7.32           |

✅ FireDucks shows major speedups in read and groupby stages.

---

## 🚀 Quick Start

```bash
pip install fireducks
```

```python
import os
os.environ["FIREDUCKS_FLAGS"] = "--benchmark-mode"
import fireducks.pandas as pd  # Just like Pandas!
```

---


