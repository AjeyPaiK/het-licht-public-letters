# Het Licht Public Letters

This repository contains advocacy correspondence issued by Het Licht together with complete, citable evidence packs that substantiate every factual claim in each letter.

## Purpose

This repository serves as a transparent, verifiable record of advocacy work, providing:
- **Complete evidence packs** for every factual claim
- **Primary source documents** including court orders, government notices, and demographic datasets
- **Reproducible calculations** with step-by-step methodology
- **Data integrity verification** through cryptographic hashes

## Repository Structure

```
het-licht-public-letters/
├── letter-[date]-[topic]/              # Individual evidence packs
│   ├── datasets/                       # Census data, demographic reports
│   ├── legal/                          # Court orders, tribunal decisions
│   ├── site-docs/                      # RTI responses, government notices
│   ├── methodology.md                  # Step-by-step verification guide
│   └── README_hashes.txt              # Cryptographic integrity checks
└── README.md                          # This file
```

## Evidence Packs

Each letter in this repository includes a complete evidence pack containing:

- **Primary source documents** that support every factual claim
- **Step-by-step methodology** for reproducing calculations
- **Data integrity verification** through cryptographic hashing
- **Citable references** with specific file paths and page numbers

## Verification Process

### 1. Data Integrity Check
Verify that files haven't been tampered with:
```bash
cd letter-[date]-[topic]
sha256sum -c README_hashes.txt
```

### 2. Step-by-Step Verification
Follow the detailed methodology in `methodology.md` to reproduce every calculation:
- Open primary source documents
- Follow documented calculation procedures
- Verify final results against claims

### 3. Source Document Access
All primary sources are either:
- **Included** in the repository
- **Publicly accessible** through official websites, portals, or RTI responses
- **Citable** with specific file references and page numbers

## Evidence Categories

| Category | Contents | Examples |
|----------|----------|----------|
| **Legal Documents** | Court orders, tribunal decisions, statutory policies | High Court judgments, NGT orders, Supreme Court decisions |
| **Demographic Data** | Census tables, population surveys, beneficiary lists | Census data, government surveys, official lists |
| **Government Records** | RTI responses, official notices, administrative orders | District orders, panchnamas, official memos |
| **Methodology** | Calculation spreadsheets, verification steps | Step-by-step guides, statistical derivations |

## Usage Guidelines

### For Researchers
1. Start with `methodology.md` for verification procedures
2. Use `README_hashes.txt` to verify data integrity
3. Follow the folder structure to locate specific evidence
4. Cite specific files and page numbers in your work

### For Journalists
1. Review the methodology for understanding data sources
2. Verify calculations using the step-by-step guides
3. Access primary documents for independent fact-checking
4. Use the evidence pack to support investigative reporting

### For Advocates
1. Use court orders and legal documents for litigation
2. Reference demographic data for policy advocacy
3. Cite government records for administrative challenges
4. Leverage the complete evidence chain for transparency

## Contributing

This repository follows strict standards for evidence-based advocacy:
- All claims must be supported by primary source documents
- Calculations must be reproducible using publicly available data
- File integrity is maintained through cryptographic hashing
- Methodology is documented step-by-step for independent verification

## Contact

For questions about the evidence packs or methodology, please refer to the specific letter folders and their accompanying documentation.

---

*This repository demonstrates the importance of transparency in advocacy work by providing complete, verifiable evidence for every factual claim.*
