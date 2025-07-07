# Methodology – derivation of household counts and religion shares  
*(folder `letter-2025-07-nos-demolitions/`, last updated 04-07-2025)*  

This note documents, file-by-file, how every numeric claim in the NOS letter can
be verified.  All raw numbers come from primary documents already stored in
this folder tree, or from openly accessible court/census/RTI sources that any
third party can obtain without payment.

---

## Folder map

| Folder | Contents |
|--------|----------|
| **datasets/** | Census tables & national eviction report |
| **legal/** | Court & tribunal orders, statutory policies |
| **site-docs/** | RTI lists, eviction notices, demolition memos |

Abbreviations – HC = High Court, SC = Supreme Court, NGT = National Green Tribunal,  
DDA = Delhi Development Authority, LDA = Lucknow Development Authority.

---

## 1  Kukrail / Akbar Nagar, Lucknow (U.P.)

| Step | File | Action | Result |
|------|------|--------|--------|
| 1 | `legal/kukrail_hc_order_06032024.pdf` (356-page HC compilation)* | Open **Annexure A – “List of dwelling units / LDA survey”** (pp ≈ 281-337). | 1 689 rows: **1 063 M** (Muslim) • **626 H/HD** (Hindu / Hindu-Dalit) |
| 2 | Divide each count by 1 689. | **63 % Muslim / 37 % Hindu-Dalit** |

\* If only the 51-page order-sheet is present, retrieve the compilation as
detailed in `legal/README_kukrail_compilation.txt`.

---

## 2  Madrasi Camp, Jangpura (Delhi)

| Step | File | Action | Result |
|------|------|--------|--------|
| 1 | `legal/jangpura_hc_order_09052025.pdf` | ¶ 26 gives **370 jhuggis** (religion not recorded). | Base count = 370 |
| 2 | `datasets/census_tn_religion_2011.pdf` | Tamil-Nadu shares: **87 % H / 6 % C / 6 % M**. | |
| 3 | Impute cluster composition (Tamil migrant settlement). | ≈ 322 H • 22 C • 22 M ⇒ **87 % H / 6 % C / 6 % M** |

---

## 3  Jailorwala Bagh, Ashok Vihar (Delhi)

| Step | File | Action | Result |
|------|------|--------|--------|
| 1 | `site-docs/dda_jailorwala_beneficiary_list.pdf` | Merge **1 078 eligible** + **567 ineligible** tables (column “Religion”). | Total 1 645 rows |
| 2 | Count by religion. | **905 H (55 %) • 576 M (35 %) • 164 Other (10 %)** |

---

## 4  Rabupura, Jewar (U.P.)

| Step | File | Action | Result |
|------|------|--------|--------|
| 1 | `site-docs/rabupura_panchnama_31052025.pdf` | Panchnama lists **40 households** (no religion). | Total = 40 |
| 2 | `datasets/census_rabupura_2011.html` | Village shares: **92 % H / 7 % M / 1 % Other**. | |
| 3 | Apply shares to 40 HH. | ≈ 37 H • 3 M ⇒ **92 % H / 7 % M** |

---

## 5  Haridwar Kanwar-route clearance (non-Muslim example)

*File*: `site-docs/haridwar_dm_order_30062025.pdf` – DM order clearing  
≈ 200 illegal shops on a Hindu-pilgrimage route.  Order text contains no
religion column but locality is Hindu-majority; cited only as evidence of
non-selective enforcement.

---

## 6  Bet Dwarka coastal clearance (mixed-community example)

*File*: `site-docs/gujhc_bet_dwarka_order_04022025.pdf` – Gujarat HC judgment
upholding demolition of unauthorised structures belonging to multiple
communities.  Religion ratios not used in headline stats.

---

## 7  National trend statistic

*File*: `datasets/hlrn_forced_evictions_2022_23.pdf`, pp 19-20 – verified
religion cases in 2022-23:

* **44 % Muslim families**  
* **56 % Hindu, Dalit, Adivasi, Other families**

---

## Verification at a glance

| Figure in letter | How to verify |
|------------------|--------------|
| 63 % / 37 % (Kukrail) | Count rows in Annexure A of HC compilation. |
| 87 % / 6 % / 6 % (Jangpura) | 370 × Tamil-Nadu census shares. |
| 55 % / 35 % / 10 % (Jailorwala) | Count religion column in DDA lists. |
| 92 % / 7 % (Rabupura) | 40 × village census shares. |
| 44 % / 56 % (National) | Read HLRN table directly. |

---

### Integrity check

Run

```bash
sha256sum -c README_hashes.txt