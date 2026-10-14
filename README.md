# SPACEPY

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-space_aerotech-lightgrey)

> Anticloud-hardened packaging of the upstream project `SPACEPY` in category **SPACE AEROTECH**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SPACE AEROTECH · **Upstream:** https://github.com/spacepy/spacepy · **Upstream pin:** `6a9f0827005c03cbc59557def78bbc035a97bbea` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3252523.svg)](https://doi.org/10.5281/zenodo.3252523)
[![Build Status](https://github.com/spacepy/spacepy/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/spacepy/spacepy/actions?query=workflow%3ACI)

# SpacePy

SpacePy is a package for Python, targeted at the space sciences, that aims to make basic data analysis, modeling and visualization easier. It builds on the capabilities of the well-known NumPy and MatPlotLib packages. Publication quality output direct from analyses is emphasized among other goals:

 - Quickly obtain data
 - Read (and write) data from (and to) data formats like NASA CDF and HDF5
 - Create publications quality plots
 - Perform complicated analysis easily
 - Run common empirical models
 - Change coordinates and time systems effortlessly
 - Harness the power of Python

The SpacePy project seeks to promote accurate and open research standards by providing an open environment for code development. In the space physics community there has long been a significant reliance on proprietary languages that restrict free transfer of data and reproducibility of results. By providing a comprehensive, open-source library of widely-used analysis and visualization tools in a free, modern and intuitive language, we hope that this reliance will be diminished.

To help foster an open and welcoming environment, we have adopted a [code of conduct](https://github.com/spacepy/spacepy/blob/main/code-of-conduct.md) that we encourage members of the SpacePy community to read and follow.

## Getting SpacePy

Our latest release version is available through PyPI and can be installed using

```
pip install spacepy --user
```

This will also automatically install most dependencies.

The latest "bleeding-edge" source code is available from our github project at [https://github.com/spacepy/spacepy](https://github.com/spacepy/spacepy).

Further installation documentation, including building from source and OS-specific information, can be found [here](https://spacepy.github.io/install.html). Full documentation is at [https://spacepy.github.io](https://spacepy.github.io).

SpacePy supports Python 3.7 and later.

### Dependencies

SpacePy has a number of well-maintained dependencies which are automatically installed by ```pip```. These include:

 - numpy (>=1.15.1)
 - dateutil (>=2.5)
 - scipy (>=1.0)
 - matplotlib (>=3.1)
 - h5py (>=2.10)

## Attribution

When publishing research which used SpacePy, please provide appropriate credit to the SpacePy team via citation or acknowledgement.

To cite SpacePy in publications, please cite both the code (DOI: 10.5281/zenodo.3252523) and the papers describing the package (BibTeX code):

```
@article{niehof2022spacepy,
  title={The SpacePy space science package at 12 years},
  author={Niehof, Jonathan T and Morley, Steven K and Welling, Daniel T and Larsen, Brian A},
  journal={Frontiers in Astronomy and Space Sciences},
  volume={9},
  year={2022},
  doi={10.3389/fspas.2022.1023612},
  publisher={Frontiers}
}
```

and/or

```
@INPROCEEDINGS{spacepy11,
author = {{Morley}, S.~K. and {Koller}, J. and {Welling}, D.~T. and {Larsen}, B.~A. and {Henderson}, M.~G. and {Niehof}, J.~T.},
title = "{Spacepy - A Python-based library of tools for the space sciences}",
booktitle = "{Proceedings of the 9th Python in science conference (SciPy 2010)}",
year = 2011,
address = {Austin, TX}
}
```

For additional information, see the [CITATION.cff](https://github.com/spacepy/spacepy/blob/main/CITATION.cff) file.
Certain modules may provide additional citations in the ```__citation__``` attribute. Contact a module's author before publication or public presentation of analysis performed by that module. This allows the author to validate the analysis and receive appropriate credit for his or her work.

For acknowledging SpacePy, please provide the URL to our github project: [github.com/spacepy/spacepy](https://github.com/spacepy/spacepy).

## Changes
Changes in the released version of SpacePy are provided in the [release notes](https://spacepy.github.io/release_notes.html). For changes since the latest release, see the [project version](https://github.com/spacepy/spacepy/blob/main/Doc/source/release_notes.rst).

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Python** (manifests: pyproject.toml, requirements.txt; scanned in UPSTREAM_CLONE)
- Top-level source layout: `Doc/`, `developer/`, `scripts/`, `spacepy/`, `tests/`
- Snapshot size: **294 files**, **49341 lines of code** (measured; see Benchmarks)
- Primary languages: `.py` (75), `.f` (58), `.par` (45), `.rst` (30), `.txt` (29), `.inc` (7)
- Upstream commit pinned for this packaging: `6a9f0827005c03cbc59557def78bbc035a97bbea`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -e .                                     # or: pip install -r requirements.txt
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

```sh
python -m spacepy    # module entry point, when the package layout matches
```

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `SPACEPY` source tree vendored in `UPSTREAM_CLONE/` (Python ecosystem). Public entry points:

- Source modules: `Doc/`, `developer/`, `scripts/`, `spacepy/`, `tests/`
- The snapshot declares 14 dependency references across 1 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Python |
| Manifests detected | pyproject.toml, requirements.txt |
| Files in snapshot | 294 |
| Lines of code | 49341 |
| Dependency references | 14 |
| Dependencies by ecosystem | pypi: 14 |
| Upstream license | No license file present in the upstream snapshot |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| pypi | numpy | >=1.15.1 | pyproject.toml |
| pypi | scipy | >=1.0 | pyproject.toml |
| pypi | matplotlib | >=3.1 | pyproject.toml |
| pypi | h5py | >=2.10 | pyproject.toml |
| pypi | python_dateutil | >=2.5 | pyproject.toml |
| pypi | -std | =legacy | setup.py |
| pypi | -mmacosx-version-min | ={min_os_ver} | setup.py |
| pypi | --print-file-name | ={f}.dylib | setup.py |
| pypi | numpy | >=1.15.1 | setup.py |
| pypi | scipy | >=1.0 | setup.py |
| pypi | matplotlib | >=3.1 | setup.py |
| pypi | h5py | >=2.10 | setup.py |
| pypi | python_dateutil | >=2.5 | setup.py |
| pypi | pandas | >=0.18 | setup.py |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

To help foster an open and welcoming environment, we have adopted a [code of conduct](https://github.com/spacepy/spacepy/blob/main/code-of-conduct.md) that we encourage members of the SpacePy community to read and follow.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `SPACEPY` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: No license file present in the upstream snapshot** (evidence: `LICENSE.md` in the upstream snapshot).

License file excerpt:

```text
Copyright 2010 Triad National Security, LLC

1. This LICENSE AGREEMENT is between Triad National Security, LLC ("Triad"),
   and the Individual or Organization ("Licensee") accessing and otherwise
   using SpacePy software in source or binary form and its associated
   documentation.

2. Subject to the terms and conditions of this License Agreement, Triad
   hereby grants Licensee a nonexclusive, royalty-free, world-wide license
   to reproduce, analyze, test, perform and/or display publicly, prepare
   derivative works, distribute, and otherwise use SpacePy alone or in any
   derivative version, provided, however, that Triad's License Agreement and
   Triad's notice of copyright, i.e., "Copyright (c) 2010 Triad National
   Security, LLC; All Rights Reserved" are retained in SpacePy alone or in any
   derivative version prepared by Licensee.

3. In the event Licensee prepares a derivative work that is based on or 
   incorporates SpacePy or any part thereof, and wants to make the derivative
   work available to others as provided herein, then Licensee hereby agrees to
   include in any such work a brief summary of the changes made to SpacePy.
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original No license file present in the upstream snapshot terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `No license file present in the upstream snapshot` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `SPACEPY` (category: SPACE AEROTECH)
- **Upstream URL:** https://github.com/spacepy/spacepy
- **Pinned commit (SHA):** `6a9f0827005c03cbc59557def78bbc035a97bbea`
- **Branch:** main
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`72262d756e4a4abdd289ef19504ad27ef67d67231f177a82337a5762c17a2911`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

