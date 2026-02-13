# Analysis Citation Keys

用于 `analysis/` 下文档快速引用，BibTeX 文件见：`analysis/refs/references.bib`。

## Standards / Specs
- `nist2024fips203` → FIPS 203 (ML-KEM)
- `kyber2021spec` → CRYSTALS-Kyber v3.02 specification
- `nistpqcround3` → NIST PQC Round 3 submissions page

## Assumptions / Reductions
- `regev2005lwe` → LWE foundational paper
- `regev2009lwesurvey` → LWE survey note
- `lyubashevsky2010ringlwe` → Ring-LWE foundational paper
- `langlois2013module` → Module-lattice reduction paper

## Parameter / Estimation
- `pqcrystalssecurityestimates` → official security-estimates repo
- `albrecht2020estimateall` → ePrint: Estimate all the {LWE, NTRU} schemes!
- `latticeestimatorrepo` → lattice-estimator repo

## Attack Surface / Implementation
- `peikert2016decade` → lattice crypto decade survey
- `pqcrystalskyberpage` → official Kyber page
- `pqcrystalskyberrepo` → Kyber reference implementation repo
- `nistpqcproject` → NIST PQC project page

> 建议：在正文使用统一格式，例如 `[@nist2024fips203]` / `\cite{nist2024fips203}`，并保持 key 在 `basics/` 与 `analysis/` 间一致。
