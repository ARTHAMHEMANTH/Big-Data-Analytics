# Pyspark Even Number Filter
## 🔹 Visual Representation of Data Flow

Original List
───────────────
[12, 7, 34, 89, 42, 55, 68, 91, 2, 77, ...]

          │
          ▼
  ┌─────────────────────┐
  │ Parallelize into RDD│
  │ numbers_rdd         │
  └─────────────────────┘
          │
          ▼
  ┌─────────────────────┐
  │ Filter Even Numbers │
  │ even_numbers_rdd    │
  └─────────────────────┘
          │
          ▼
  ┌─────────────────────┐
  │ Collect & Display   │
  │ even_numbers        │
  └─────────────────────┘
          │
          ▼
Filtered Even Numbers
───────────────
[12, 34, 42, 68, 2, ...]
