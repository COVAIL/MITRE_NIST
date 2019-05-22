![alt text](https://github.com/ColumbusCollaboratory/MITRE_NIST/blob/master/cclogo.png) 
# A Crowdsourcing Exchange for mapping various sources of Information security vulnerabilities, exposures, threats, and controls data

## What are you asking?

The [Columbus Collaboratory](https://columbuscollaboratory.com/) is asking the community to help us create mappings from CWE (common weakness enumeration) to NIST 800-53r4 moderate controls using our initial mapping formula.


## Why are you asking?

The Collaboratory team is trying to surface correlations and semantic relationships between available sources of information security vulnerabilities and exposures to attack types so we can better understand how attackers think about exploiting them.  By also relating controls sets like NIST 800-53 we hope to give cybersecurity teams comprehensive, threat-informed information that can help them manage and mitigate risk in various parts of their program.

## How to get started?

The Collaboratory team in their analytical approach has focused on the relationships between the following data sets:
-	NVD
-	CWE
-	CVE
-	CAPEC
-	ATT&CK Technique
-	NIST SP 800-53r4 moderate

Below is our data model and a sample of the “mashup”.  We have found that relating CVE, CWE, CAPEC, and ATT&CK technique to be fairly repeatable and programmatic whereas relating the controls set to be more challenging and manual.  We have chosen to crowdsource this aspect of the analysis and below is the initial mapping formula to guide your analysis.


![alt text](https://github.com/ColumbusCollaboratory/MITRE_NIST/blob/master/datamodel.PNG) 

CVE	|CWE ID	|CWE Name	|CAPEC ID|	CAPEC Name	|ATT&CK Technique Name	|ATT&CK Technique ID	|NIST SP 800-53r4
---	|-----	|--------	|--------|	------------|-----------------------|---------------------|----------------
CVE-2017-9788|CWE-20|Improper Input Validation|CAPEC-312	|Active OS Fingerprinting	|System Information Discovery|T1082|	 AT-3(3), SI-2, SI-11|
CVE-2018-17082|CWE-79|Cross-Site Scripting|CAPEC-63|Cross-Site Scripting (XSS)|Drive-by Compromise|T1189	|AT-3(3), SI-2, SI-10
CVE-2017-9798|CWE-416|Use After Free|CAPEC-312|Active OS Fingerprinting|System Information Discovery|T1082|IA-5

## Example Use Cases

To help illustrate a practical application for this mapping exercise we have included the following examples of a few common attacks and corresponding security controls that could be used to protect potential vulnerabilities from being exploited:

1. Password Spraying – a password spray attack is simply enumerating a list of users from an organization and “spraying” commonly used passwords against that list in an effort to “brute force” or crack a password of an account in order to gain unauthorized, but authenticated access to an organization.

  Keywords: password blacklisting; commonly used, breach data; multi-factor	

  NIST controls: AC-12; AU-2; IA-2; IA-5 (1),(2), (4), (8), (10), (12); SI-11

2. Malware replication – malware is malicious or infected code that actively replicates itself throughout your network. It can persist in the shape of a virus, spyware, worm, trojan, or ransomware.

  Keywords: malicious code, mobile code, malware replication, code execution, network segmentation, shared admin 

  NIST controls: AC-4 (14); AC-6 (8) (10); AC-19; AT-2; AT-3(4); CM-10; IA-2(11); IR-6; IR-10; MA-3(2); MP-6(3); PL-8(2); SA-12(7); SA-19; SC-5; SC-7(9); SC-18 (1-5); SC-3(3); SC-34(1); SC-35; SC-37; SC-43; SC-44;SI-3 (1-10); SI-4 (24)

3. Network Access Control (NAC) bypass – wireless intruders can bypass 802.1x network access controls by sniffing network traffic with a man-in-the-middle attack/device, thus enabling the capture and ultimately spoofing of hardware Media Access Control (MAC) addresses of approved network devices to then emulate those devices on a local network.


## Contribution Guidelines

Please ensure your pull request adheres to the following guidelines:

- Alphabetize your entry.
- Search previous suggestions before making a new one, as yours may be a duplicate.
- Make an individual pull request for each suggestion.
- New categories, or improvements to the existing categorization are welcome.
- Keep descriptions short and simple, but descriptive.
- Start the description with a capital and end with a full stop/period.
- Check your spelling and grammar.
- Make sure your text editor is set to remove trailing whitespace.

Thank you for your suggestions!

## Versioning
1.0
## Authors
Gina Greco, 
Jody Denner,
Brandon Ritze,
Brandon Gale,
Troy Vennon,
Amanda Vu
## License

This project is licensed under Creative Commons (CC)

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)

## Acknowledgments
Jeff Schmidt, NIST, MITRE


