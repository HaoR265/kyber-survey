# Basics References

本目录收集“进入 ML-KEM / Kyber 之前”的基础参考材料（链接）

---

## 0. Standards / Specs（标准与规格）
- NIST FIPS 203 — ML-KEM 标准（最终版 PDF / 标准页）
  - PDF: https://nvlpubs.nist.gov/nistpubs/fips/nist.fips.203.pdf
  - Page: https://csrc.nist.gov/pubs/fips/203/final
- CRYSTALS-Kyber Specification v3.02（Round-3 规格书）
  - PDF: https://pq-crystals.org/kyber/data/kyber-specification-round3-20210804.pdf

---

## 1. Surveys / Overviews（综述：先建立全景）
- C. Peikert — *A Decade of Lattice Cryptography*（格密码十年综述）
  - Publisher page: https://www.nowpublishers.com/article/DownloadSummary/TCS-074

---

## 2. Core Assumptions（核心问题：LWE / 最坏到平均）
- O. Regev — *On Lattices, Learning with Errors, Random Linear Codes, and Cryptography*（LWE 基础论文：最坏到平均的核心之一）
  - PDF: https://cims.nyu.edu/~regev/papers/qcrypto.pdf
- O. Regev — *The Learning with Errors Problem*（LWE 综述讲义）
  - PDF: https://cims.nyu.edu/~regev/papers/lwesurvey.pdf
- D. Micciancio & O. Regev — *Worst-case to Average-case Reductions based on Gaussian Measures*（高斯测度路线的最坏到平均）
  - PDF: https://cims.nyu.edu/~regev/papers/average.pdf

---

## 3. Lattice Algorithms（算法工具：SVP/CVP/LLL 语言来源）
- 了解 LLL 的经典背景（SVP/LLL 的基础文档入口）
  - PDF（讲 SVP/LLL 的材料入口之一）: https://www.zib.de/userpage//groetschel/Bilder/L3.pdf
- LLL 的更现代/教学型讲解（可选）
  - arXiv: https://arxiv.org/abs/2410.22196

---

## 4. Structured LWE（环/模：走向 Ring-LWE / Module-LWE 的桥）
- V. Lyubashevsky, C. Peikert, O. Regev — *On Ideal Lattices and Learning with Errors over Rings*（Ring-LWE 经典论文）
  - PDF: https://scispace.com/pdf/on-ideal-lattices-and-learning-with-errors-over-rings-nu7g19xlwr.pdf
- A. Langlois et al. — *Worst-Case to Average-Case Reductions for Module Lattices*（模块格/模块相关 reductions）
  - PDF: https://perso.ens-lyon.fr/damien.stehle/downloads/MSIS.pdf

---

## 5. Notes Link
- 基础笔记：`basics/` 下自行新建
- 如果某条文献对应到更深的分析/工程，再在 `analysis/` 或 `engineering/` 的 refs 里重复登记一次。


## 6. Citation Files
- BibTeX: `basics/refs/references.bib`
- Citation keys: `basics/refs/KEYS.md`
