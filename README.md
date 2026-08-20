## Luis Fidel Castellanos Diaz

Independent software assurance and security research focused on legacy
systems, cryptographic integrity, forensic analysis, and reproducible
technical evidence.

---

### Active Projects

| Repository | Description |
|---|---|
| [cobol-shield](https://github.com/LuisCastellanos-dev/cobol-shield) | Static analysis toolkit for COBOL legacy systems — invisible Unicode detection, format boundary analysis, source transformation integrity |
| [vtr-forensic-img](https://github.com/LuisCastellanos-dev/vtr-forensic-img) | Hybrid Rust+Python forensic image analysis — binary parsing, chain of custody, adversarial test suite |
| [cryptofault](https://github.com/LuisCastellanos-dev/cryptofault) | Passive PCAP and certificate analysis for OT/ICS — TLS version detection, weak keys, plaintext sessions |
| [cfg-shield](https://github.com/LuisCastellanos-dev/cfg-shield) | Feature flag semantic drift detector for Rust — confirmed against generic-ecies |

---

### Upstream Contributions

- **FreeBSD** — crp/mbuf/refcount leak fix in `sys/net/if_ovpn.c` — [rGa841961da752](https://cgit.freebsd.org/src/commit/?id=a841961da752) — merged by kp (Kristof Provost)
- **RustCrypto/crypto-bigint** — documentation clarification for `xgcd_vartime` delegation — [PR #1333](https://github.com/RustCrypto/crypto-bigint/pull/1333)
- **IBM/Bank-of-Z** — copy-paste defect in ABND-TIME seconds field across 23 CICS programs — [PR #210](https://github.com/IBM/Bank-of-Z/pull/210) open, linked to [issue #205](https://github.com/IBM/Bank-of-Z/issues/205)
- **generic-ecies** — SharedInfo1/2 analysis per SEC 1 v2.0 §5.1.3 — [issue #2](https://github.com/nickel-lang/generic-ecies/issues/2), PR in preparation

---

### Published Research

- *Source Transformation Integrity in Legacy COBOL Systems* — [DOI 10.5281/zenodo.21973424](https://doi.org/10.5281/zenodo.21973424) — Zenodo, 2026, CC BY 4.0

---

### Methodology

Each project distinguishes observed facts from inference and projection.
Security claims require a reproducible artifact — hexdump -C, not visual render.
