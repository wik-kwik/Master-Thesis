# Malware Analysis & Digital Forensics

This repository contains the materials and results associated with my Master's thesis:

**“Evaluation of Selected Digital Forensics Tools in Terms of Data Analysis”**

The thesis examines how malware analysis and digital forensics can be combined to investigate malicious software, understand its behavior, reconstruct system activity, and identify the digital artifacts left on compromised machines.

## Research Scope

The project covers three complementary areas:

### Static Malware Analysis

Examining suspicious files without executing them, including:

- file hash calculation and reputation checks,
- string extraction,
- Portable Executable inspection,
- identification of suspicious indicators,
- rule-based malware detection with YARA.

Tools used include **Microsoft Strings, VirusTotal, CFF Explorer, and YARA**.

### Dynamic Malware Analysis

Observing malware behavior during controlled execution, including:

- network communication,
- registry modifications,
- process activity,
- file-system changes.

The analysis uses tools such as **FakeNet-NG, Regshot, and Process Monitor**.

### Digital Forensics

Investigating system artifacts and reconstructing activity through:

- memory-dump analysis,
- process and network-connection examination,
- suspicious file identification and extraction,
- endpoint artifact collection,
- network-wide threat hunting.

The evaluated tools include **Volatility and Velociraptor**.

## Analysis Environment

All experiments were conducted in an isolated, nested virtual-machine environment. Separate virtual machines were prepared for malware analysis and digital-forensic investigation, with **FLARE VM** providing the primary Windows malware-analysis toolkit.

The environment was designed to reduce the risk of malware escaping or communicating with external systems.

## Key Findings

The research demonstrates that no single tool provides a complete view of a security incident.

Static analysis supplies initial indicators and information about a suspicious file. Dynamic analysis reveals its runtime behavior and system interactions. Digital-forensic tools add the broader context required to reconstruct events and examine artifacts in memory, processes, files, and endpoint data.

Combining these methods therefore produces a more complete and reliable understanding of malicious activity.

## Thesis

The complete Master's thesis is included in this repository as a PDF:

**Evaluation of Selected Digital Forensics Tools in Terms of Data Analysis**

## Disclaimer

The malware samples and techniques presented in this repository are provided exclusively for educational and research purposes.

All malware analysis was performed in an isolated and controlled virtual environment. Do not execute malware samples on production systems, personal devices, or networks that are not specifically designed for security research.
