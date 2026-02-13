# Analysis References

本目录收集 `analysis/` 对应主题的核心参考文献与资料链接（安全性分析、参数对比、标准差异、实现安全结论）。

---

## 0. Standards / Primary Specs（标准与一手规格）
- NIST FIPS 203 — *Module-Lattice-Based Key-Encapsulation Mechanism Standard (ML-KEM)*
  - PDF: https://nvlpubs.nist.gov/nistpubs/fips/nist.fips.203.pdf
  - Page: https://csrc.nist.gov/pubs/fips/203/final
- CRYSTALS-Kyber Specification v3.02（Round-3 规格书）
  - PDF: https://pq-crystals.org/kyber/data/kyber-specification-round3-20210804.pdf
- NIST PQC Round 3 Submissions（Kyber 提交材料入口）
  - Page: https://csrc.nist.gov/projects/post-quantum-cryptography/round-3-submissions

---

## 1. Security Assumptions / Proof Context（安全假设与证明背景）
- O. Regev — *On Lattices, Learning with Errors, Random Linear Codes, and Cryptography*
  - PDF: https://cims.nyu.edu/~regev/papers/qcrypto.pdf
- O. Regev — *The Learning with Errors Problem*
  - PDF: https://cims.nyu.edu/~regev/papers/lwesurvey.pdf
- V. Lyubashevsky, C. Peikert, O. Regev — *On Ideal Lattices and Learning with Errors over Rings*
  - PDF: https://scispace.com/pdf/on-ideal-lattices-and-learning-with-errors-over-rings-nu7g19xlwr.pdf
- A. Langlois et al. — *Worst-Case to Average-Case Reductions for Module Lattices*
  - PDF: https://perso.ens-lyon.fr/damien.stehle/downloads/MSIS.pdf

---

## 2. Parameter & Concrete Security Estimation（参数与具体安全估计）
- pq-crystals/security-estimates（Kyber 官方安全估计脚本仓库）
  - Repo: https://github.com/pq-crystals/security-estimates
- Martin R. Albrecht et al. — *Estimate all the {LWE, NTRU} schemes!*
  - ePrint: https://eprint.iacr.org/2020/055
- lattice-estimator（LWE/RLWE 具体攻击代价估算常用工具）
  - Repo: https://github.com/malb/lattice-estimator

---

## 3. Attacks, Failure Probability, Decryption Behavior（攻击面与失败概率）
- C. Peikert — *A Decade of Lattice Cryptography*（综述）
  - Publisher page: https://www.nowpublishers.com/article/DownloadSummary/TCS-074
- Kyber 官方资源页（集中包含论文、实现、说明）
  - Page: https://pq-crystals.org/kyber/
- 说明：
  - 针对“失败概率 / 去密钥失败驱动的攻击”与“CCA 转换相关边界”分析时，优先回到 FIPS 203 与 Kyber v3.02 的原始定义，再补充近期论文。

---

## 4. Side-channel / Fault（侧信道与故障）
- pq-crystals/kyber（参考实现，用于定位实现层面的泄漏面）
  - Repo: https://github.com/pq-crystals/kyber
- NIST IR 相关实现指南与迁移建议入口（PQC 项目页）
  - PQC project page: https://csrc.nist.gov/projects/post-quantum-cryptography
- 说明：
  - 侧信道/故障文献更新快，建议在 `analysis/` 各专题文档里按攻击类型（timing/cache/power/fault）单独维护小型 refs 子清单。

---

## 5. Standard Difference Tracking（标准差异追踪）
- FIPS 203（最终规范）
  - PDF: https://nvlpubs.nist.gov/nistpubs/fips/nist.fips.203.pdf
- Kyber v3.02（设计与说明）
  - PDF: https://pq-crystals.org/kyber/data/kyber-specification-round3-20210804.pdf
- 追踪建议：
  - 在分析文档中固定使用“章节号 + 术语表”记录差异（如 API 命名、编码细节、参数命名与取值）。

---

## 6. Notes Link
- 分析主入口：`analysis/README.md`
- 若某篇文献被深入复盘，可在 `notes/` 新建对应读书笔记，并在分析文档中回链。


## 7. Citation Files
- BibTeX: `analysis/refs/references.bib`
- Citation keys: `analysis/refs/KEYS.md`
