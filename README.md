# Phishing-Investigation

**Summary**

A phishing attempt impersonating the e-commerce platform Allegro was analysed for this investigation. The email directed users to a suspicious domain designed to mimic Allegro, an e-commerce platform. 

Further analysis of the URL contained within the email using VirusTotal found characteristics consistent with credential harvesting and it had been judged as malicious by 13 security vendors.

The domain shows indicators of impersonation and social engineering, meant to deceive users into giving up sensitive details. This type of attack is commonly used to get unauthorised access via the details gathered.

This has therefore been classified as a phishing attempt. The URL should be blocked and users who may have interacted with it should be advised to reset credentials and enable multi-factor authentication.

**Objective**

The objective of this investigation was to analyse a suspected phishing email impersonating the Allegro platform and determine whether the URL contained within the email was malicious.

The investigation focused on finding indicators of compromise, validating the legitimacy of the domain using VirusTotal, and assessing risk to users.

**Methodology**

The investigation followed a Tier 1 SOC workflow 

1. The initial email was reviewed to find indicators of social engineering, such as brand impersonation and external links
2. The URL embedded in the email was extracted and analysed to check legitimacy
3. The domain was evaluated using VirusTotal to check its reputation among security vendors
4. Based on the evidence, it was deemed to be in line with common phishing patterns.

**Analysis**

The initial email was designed to impersonate an email from the Allegro platform. It was attempting to gain user trust and encourage them to click a malicious link.

The URL (*allegro.126325g2.sbs*) demonstrates characteristics associated with phishing infrastructure:

1. It contains the term "allegro", in an attempt to imitate the platform
2. The use of a random selection of characters ("126325g2") appears to be automatically generated
3. The 'sbs' domain is cheap and therefore often used for malicious use cases. It is identified as a high-risk top level domain.

The URL was analysed using VirusTotal to determine reputation among security vendors. This analysis found 13 security vendors had deemed it malicious. Screenshots of the VirusTotal display are added to the repo.

**Conclusion**

The investigation determined that the email and the associated link were consistent with a phishing campaign. This was determined from analysis of the embedded URL.

Based on the findings the domain should be treated as malicious and blocked. Users who clicked the link will need to change their credentials and add multi-factor authentication. I would also recommend users be given training on how to spot phishing attacks.

