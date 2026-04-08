# Governance-Risk-Compliance-for-MBTA
This project contains data classification and policies designed for a Transportation system portal.

MBTA myCharlie Portal

Author: Utkarsha Shirole

Organization: Massachusetts Bay Transportation Authority (MBTA)

System in Scope: myCharlie Web Portal (mycharlie.mbta.com)

Effective Date: March 2026

**About This Project**
This project is a security policy suite built for the MBTA's myCharlie web portal, a public-facing platform used by Massachusetts riders to purchase passes, manage CharlieCards, set up Autopay, and access reduced-fare programs. The portal handles a sensitive mix of data including customer PII, payment card information, disability documentation, and state assistance enrollment records. That combination results in a HIGH overall system impact level under FIPS 199, making a structured, documented security posture a regulatory necessity alongside frameworks like PCI DSS and FTA requirements.
The suite covers data classification, risk categorization, vendor governance, and business continuity, each written to be actionable by the teams responsible for carrying them out.


**Information Security Policy**
The governing document for MBTA's information security program. It establishes the data classification framework (Confidential, Restricted, Public), organizational responsibilities across Executive Management, CISO, and IT, and sets the foundation that all other policies in this suite build on.

**Risk Categorization**
A FIPS 199 security categorization of the myCharlie portal using the NIST SP 800-60 information type taxonomy. It formally determines the system's sensitivity across five information types and concludes:

SC (myCharlie Portal) = {(Confidentiality, HIGH), (Integrity, MODERATE), (Availability, MODERATE)}

The HIGH confidentiality rating is driven by payment card data and disability/state assistance records, the latter of which constitutes both PHI and socioeconomic sensitive data.

**Business Continuity Plan**
Defines recovery strategies, escalation procedures, and fallback operations to keep the myCharlie portal running during disruptions. Covers DNS-based geographic failover, synchronous database replication, a 72-hour offline fare collection window at vending machines, and manual fallback options for riders if the portal is fully unavailable.

**Vendor Management Policy**
MBTA's Cybersecurity Supply Chain Risk Management (C-SCRM) framework governing the full vendor lifecycle from onboarding to offboarding. Defines risk tiers, assessment cadences, contract security requirements (SOC 2 Type II, breach notification within 48 hours, MFA, least-privilege access), and ongoing monitoring triggers including foreign acquisitions and TSA directive updates.
