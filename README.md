Android Security Updates – Extended Vulnerability & Exploitability Analysis

Overview

This project analyzes Android devices after they reach End-of-Life (EOL) and studies how vulnerabilities continue affecting unsupported devices over time.

Using NIST CVE data and vendor device information, the project evaluates:

* post-EOL vulnerability exposure
* exploitability characteristics
* vendor security differences
* long-term device security risks

This extended version also introduces additional security analysis features such as:

* Safe Usage Window (SUW)
* Dynamic Device Risk Score (DSRS)
* Post-EOL Exploitability Analysis

⸻

How the Project Works

1. NIST CVE Processing

The project downloads and processes vulnerability data from the NIST National Vulnerability Database (NVD).

The dataset includes:

* CVE identifiers
* vulnerability descriptions
* CVSS information
* severity levels
* attack vectors
* publication dates

The raw JSON feeds are flattened into a CSV dataset for easier analysis.

⸻

2. Vendor Device Data

Unsupported Android device information is collected for multiple vendors including:

* Samsung
* Xiaomi
* Oppo
* Google

The datasets contain:

* device names
* Android versions
* vendor information
* last supported update dates

⸻

3. Vulnerability Mapping

Devices are mapped to vulnerabilities based on their Android versions and associated CVEs.

The project then identifies:

* vulnerabilities affecting unsupported devices
* vulnerabilities appearing after EOL
* exploitability characteristics of those vulnerabilities

⸻

Novel Additions

Safe Usage Window (SUW)

The Safe Usage Window estimates how long an unsupported Android device may remain reasonably safe after vendor support ends.

Instead of only counting vulnerabilities, this feature focuses on:

* post-EOL usability
* vulnerability escalation
* practical security exposure over time

Devices with high numbers of critical vulnerabilities receive shorter safe usage estimates.

⸻

Dynamic Device Risk Score (DSRS)

The Dynamic Device Risk Score evaluates the practical exploitability risk of unsupported devices.

Unlike traditional vulnerability counting, DSRS considers:

* severity
* attack vector
* attack complexity
* user interaction requirements
* CVSS information

This helps identify devices with higher real-world attack exposure.

⸻

Post-EOL Exploitability Analysis

This addition studies how exploitable post-EOL vulnerabilities are in practice.

The analysis focuses on:

* critical vulnerabilities
* remotely exploitable vulnerabilities
* no-user-interaction vulnerabilities
* exploitability characteristics from CVE metadata

This improves the project’s cybersecurity relevance by focusing on practical attack exposure rather than only vulnerability quantity.

⸻

Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

⸻

Repository Structure

Data/
 ├── NIST-all/
 ├── Samsung/
 ├── Xiaomi/
 ├── Oppo/
 ├── Google/
Notebooks/
 ├── analysis notebooks
Scripts/
 ├── download_cve.sh

⸻

Future Improvements

Possible future extensions include:

* machine learning based risk prediction
* exploit forecasting
* hardware-specific exploitability analysis
* automated vendor patch analysis

⸻

Conclusion

This project extends traditional Android post-EOL vulnerability analysis by incorporating exploitability-aware security evaluation techniques.

The added novelty contributions transform the project from a simple vulnerability accumulation study into a more practical cybersecurity risk assessment framework capable of estimating:

* practical attack exposure
* exploitability risk
* and post-support safe operational duration.
