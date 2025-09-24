# Layout-Aware Metadata Extraction Framework

This is a theoretical documentation of the thesis research project. For executing the experiments, refer to: [CODE](./CODE.md).

## Table of contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)

## Introduction

**Motivation**

Academic publications are the cornerstone of scientific communication, yet their widespread use of PDF formats poses significant challenges for automated metadata extraction. Unlike structured formats such as XML or HTML, PDFs prioritize visual presentation over semantic structure, making it difficult to reliably capture critical bibliographic fields like titles, authors, affiliations, and DOIs.

**Overview**

This project investigates metadata extraction from scholarly PDFs by comparing two paradigms: layout-aware systems, which leverage structural and visual cues, and small-scale language models (SLMs), which rely on contextual reasoning. The work focuses on the construction of high-quality ground-truth datasets, and systematic evaluation of both approaches across accuracy, robustness, and computational efficiency.

Since accurately extracting the linear reading order of text from PDF documents is a prerequisite for downstream metadata extraction, this work also includes benchmarking of PDF parsers.

**Highlights**

* **Ground-Truth Resources** – Provides two curated datasets:
  * A page-level benchmark from DocBank for PDF parser evaluation.
  * A gold-standard collection of metadata for scholarly PDFs.
* **Parser Benchmarking** – Assesses five open-source PDF parsers on text fidelity, completeness, and logical reading order.
* **SLM Pipeline** – Demonstrates metadata extraction using prompt-engineered, schema-constrained outputs without model retraining.
* **Baseline Comparison** – Benchmarks layout-aware GROBID against SLM-based pipelines for accuracy, efficiency, and robustness.

**Metadata Fields**

Title, Authors, Affiliations, Email IDs, Publisher, Publication Date, DOI, Keywords, and Abstract.

---

## Project Overview


