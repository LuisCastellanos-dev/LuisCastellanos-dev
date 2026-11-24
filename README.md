# Luis Fidel Castellanos Diaz

Applied cryptography and systems engineering research across FreeBSD, Rust, and COBOL
ecosystems — compilation context security, cryptographic integrity, and crypto agility
for critical infrastructure. Every claim backed by a reproducible artifact —
hexdump -C, not visual render.

---

## Active Projects

| Repository | Description |
|---|---|
| [cobol-shield](https://github.com/LuisCastellanos-dev/cobol-shield) | Static analysis toolkit for COBOL legacy systems — invisible Unicode detection, format boundary analysis, source transformation integrity |
| [vtr-forensic-img](https://github.com/LuisCastellanos-dev/vtr-forensic-img) | Hybrid Rust+Python forensic image analysis — binary parsing, chain of custody, adversarial test suite |
| [cryptofault](https://github.com/LuisCastellanos-dev/cryptofault) | Passive PCAP and certificate analysis for OT/ICS — TLS version detection, weak keys, plaintext sessions |
| [cfg-shield](https://github.com/LuisCastellanos-dev/cfg-shield) | Feature flag semantic drift detector for Rust — confirmed against generic-ecies |
| [vtr-sentinel-kmod](https://github.com/LuisCastellanos-dev/vtr-sentinel-kmod) | FreeBSD 14.5 kernel module for OT/ICS security telemetry — Phase 3 confirmed, reproducible build under R-09 |
| [vtr-methodology](https://github.com/LuisCastellanos-dev/vtr-methodology) | VTR-DEV-001 and VTR-COMP-001 — artifact production and compilation context methodology, CC BY 4.0 |

---

## Upstream Contributions

- **FreeBSD** — crp/mbuf/refcount leak fix in `sys/net/if_ovpn.c` — [rGa841961da752](https://cgit.freebsd.org/src/commit/?id=rGa841961da752) — merged by kp (Kristof Provost)
- **FreeBSD** — `MPASS(hlen <= sizeof(dst.sa_data))` assertion in `sys/net/bpf_ifnet.c` — [rG599c3d7d7ae5](https://cgit.freebsd.org/src/commit/?id=rG599c3d7d7ae5) — committed by glebius
- **RustCrypto/crypto-bigint** — documentation clarification for `xgcd_vartime` delegation — [PR #1333](https://github.com/RustCrypto/crypto-bigint/pull/1333)
- **IBM/Bank-of-Z** — copy-paste defect in ABND-TIME seconds field across 23 CICS programs — [PR #210 merged](https://github.com/IBM/Bank-of-Z/pull/210), closes [Issue #205](https://github.com/IBM/Bank-of-Z/issues/205)
- **opensourcecobol4j** — security audit (15 findings), PRs #917–#921 pending upstream review; four fixes ported by the maintainer into Hagane COBOL 2.0.0 (#61 ports the null-byte check only) — [CHANGELOG](https://github.com/yutaro-sakamoto/Hagane-COBOL/blob/main/CHANGELOG.md)
- **Raspberry Pi Linux** — resource leak and stack overflow in vc04_services (VTR-RPi-001, VTR-RPi-002) — resolved in [PR #7576](https://github.com/raspberrypi/linux/pull/7576)
- **generic-ecies** — SharedInfo/1,2 analysis per SEC 1 v2.0 §5.1.3 — [Issue #2](https://github.com/LFDT-Lockness/generic-ecies/issues/2), PR in preparation
- **Tailscale** — FreeBSD port version representation divergence — [Issue #18136](https://github.com/tailscale/tailscale/issues/18136)
- **Tailscale** — Parrot OS Echo misdetected as debian bullseye in install.sh — [Issue #20960](https://github.com/tailscale/tailscale/issues/20960)

---

## Published Research

- *VTR-FINDINGS-001: Structured Evidence and Validation Contract for OT/ICS Security Findings* — [DOI 10.5281/zenodo.22821614](https://doi.org/10.5281/zenodo.22821614) — Zenodo 2026, MIT
- *Source Transformation Integrity in Legacy COBOL Systems* — [DOI 10.5281/zenodo.21974261](https://doi.org/10.5281/zenodo.21974261) — Zenodo 2026, CC BY 4.0
- *Compilation Context as a Security Variable: A Cross-Language Classification Framework* — [DOI 10.5281/zenodo.22063208](https://doi.org/10.5281/zenodo.22063208) — Zenodo 2026, CC BY 4.0

---

## Methodology

Each project distinguishes observed facts from inference and projection under the
CONFIRMED / PROBABLE / OBSERVED framework. Build reproducibility is verified under
R-09: source → toolchain → artifact → evidence, with SHA-256 at each boundary.
