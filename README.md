# Incident Response Plan & Execution (Ransomware Simulation)

**Objective**

Investigate and respond to a simulated ransomware incident affecting a Finance department workstation by applying the National Institute of Standards and Technology (NIST) Incident Response Lifecycle. The focus was on identifying affected assets, determining the scope of compromise, and executing containment recovery actions to restore operations.

**Detection & Analysis**

Initial indicators included:
- Inaccessibility of financial files
- Indicators of file encryption on a Finance workstation
- Signs of potential access to shared network resources

I analyzed the affected system and surrounding environment to:
- Identify the initial infected host
- Determine whether shared drives or additional endpoints were impacted
- Assess potential lateral movement due to lack of segmentation

This established the scope of compromise and guided containment priorities.

**Containment**

Based on the identified scope:
- The infected workstation was isolated from the network
- Access to shared Finance resources was restricted
- Systems with potential exposure paths were prioritized for containment

These actions prevent further encryption and limit the spread across interconnected systems.

**Eradication**

To remove the threat:
- The infected system was reimaged

This removes any potential malware persistence mechanisms to ensure a clean recovery state and reduce the risk of reinfection.

**Recovery**

To recover from the incident:
- Systems were restored using known-good backups
- File integrity and system functionality were validated
- Access to restored systems was reinstated
  
**Post-Incident Improvements**

Post-incident analysis identified key security gaps, leading to the following recommendations:
- Network segmentation to reduce lateral movement risk
- Enforcement of least privilege access controls
- Improved monitoring for early detection of abnormal file activity

**Analyst Decision-Making**

Key decisions made:
- Prioritized isolation over investigation delay to minimize spread
- Chose full system reimaging over selective malware removal
- Treated shared resources as potentially compromised due to a lack of segmentation
- Relied on backup restoration rather than attempting decryption

**Scenario Analysis**

A simulated ransomware incident affected a Finance department workstation, encrypting critical files. Due to limited network segmentation, there was a risk of lateral movement to shared drives and additional endpoints. The incident primarily affected data availability and required rapid scoping and containment to prevent further spread.

**Key Findings**

- Limited network segmentation increased the risk of lateral movement between systems
- Rapid isolation of infected assets significantly reduces ransomware spread
- Backup-based recovery is more reliable than attempting decryption or ransom payment
- Data availability is a primary impact of ransomware and must be prioritized in response efforts
- Defense-in-depth strategies improve resilience against similar incidents

**Skills Demonstrated**

- Incident analysis and scope of compromise assessment
- Endpoint containment and access restriction techniques
- Backup-based recovery and system restoration validation
- Application of the NIST Incident Response Lifecycle
- Identification of security gaps and recommendation of mitigation strategies

<img width="400" height="250" alt="IRLchart" src="https://github.com/user-attachments/assets/e30d6af7-a24e-40ea-a242-35c689402d81" />

- The incident response lifecycle chart visualizes how risk levels changed across each phase. Risk peaked during detection and analysis due to uncertainty in scope, then decreased significantly following containment and eradication actions. This reflects the impact of rapid isolation and controlled recovery in reducing overall incident severity.
