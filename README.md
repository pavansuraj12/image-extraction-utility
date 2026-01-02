# Image Extraction Utility

A simple Python utility to **recursively extract only image files** from datasets
with arbitrary folder depth and consolidate them into a **single flat directory**.

This tool is useful for cleaning Kaggle or real-world datasets before
model inference, testing, or analysis.

---

## ✨ Features

- Recursively scans all subfolders
- Copies **only image files**
- Flattens everything into a single destination folder
- Preserves original filenames
- Skips duplicate filenames to avoid overwriting
- Ignores all non-image files
- Safe to re-run multiple times

---

## 📁 Supported Image Formats

- `.jpg`
- `.jpeg`
- `.png`
- `.bmp`
- `.tiff`
- `.webp`

All other file types are ignored.

---

## 🎯 Use Case

This utility is designed for situations where:
- A dataset contains deeply nested folders
- Only image files are required
- The dataset needs to be flattened for:
  - YOLO / CNN inference
  - Batch testing
  - Dataset inspection
  - Rapid experimentation

---

## 🚀 Usage

### 1. Update paths in the script

Open `image_only_extractor.py` and modify:

```python
SOURCE_DIR = "/path/to/raw/dataset"
DEST_DIR = "/path/to/output/images"
