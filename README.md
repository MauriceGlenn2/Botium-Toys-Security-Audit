

# Botium Toys: Scope, Goals, and Risk Assessment Report

## Scope and Goals of the Audit
**Scope**: The scope is defined as the entire security program at Botium Toys. This includes assessing all assets, as well as internal processes and procedures related to the implementation of controls and compliance best practices.

**Goals**:  
- Assess existing assets.
- Complete the controls and compliance checklist to determine which controls and compliance best practices need to be implemented to improve Botium Toys’ security posture.


## Current Assets
### Assets Managed by the IT Department Include:
- On-premises equipment for in-office business needs.
- Employee equipment:  
  - End-user devices (desktops, laptops, smartphones)  
  - Remote workstations  
  - Headsets, cables, keyboards, mice, docking stations  
  - Surveillance cameras, etc.
- Storefront products available for retail sale (onsite and online), stored in the company’s adjoining warehouse.
- Management of systems, software, and services:  
  - Accounting  
  - Telecommunication  
  - Database  
  - Security  
  - E-commerce  
  - Inventory management
- Internet access, internal network, data retention, and storage.
- Legacy system maintenance:  
  - End-of-life systems that require human monitoring.

---

## Risk Assessment

### Risk Description:
Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all proper controls in place and may not be fully compliant with U.S. and international regulations and standards.

### Control Best Practices:
The first of the five functions of the NIST CSF is **Identify**. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they need to classify existing assets and determine the impact of the loss of those assets on business continuity.

### Risk Score:
- On a scale of 1 to 10, the risk score is **8** (fairly high).  
- This is due to a lack of controls and adherence to compliance best practices.

### Additional Comments:
- The potential impact from the loss of an asset is rated as **medium** because the IT department does not know which assets would be at risk.  
- The risk to assets or fines from governing bodies is **high** due to the lack of necessary controls and adherence to compliance regulations.

### Specific Details:

<details>
  <summary>Click here for specific details</summary>

  - All Botium Toys employees currently have access to internally stored data, including potentially sensitive cardholder data and customers' PII/SPII.
  - **Encryption** is not being used to ensure confidentiality of customers' credit card information (accepted, processed, transmitted, and stored in the internal database).
  - **Access Controls** related to least privilege and separation of duties have not been implemented.
  - The IT department ensures availability and has integrated controls to ensure data integrity.
  - A **firewall** is in place, blocking traffic based on a set of defined security rules.
  - **Antivirus software** is installed and regularly monitored.
  - There is no **Intrusion Detection System (IDS)** currently installed.
  - **Disaster recovery plans** are not in place, and there are no backups of critical data.
  - The IT department has established a plan to notify EU customers within **72 hours** in the event of a security breach. Privacy policies and procedures have also been developed.
  - The existing **password policy** is nominal and not aligned with current best practices (e.g., at least eight characters, a combination of letters, numbers, and special characters).
  - There is no centralized **password management system** to enforce the minimum password requirements.
  - **Legacy systems** are monitored but not on a regular schedule, and methods for intervention are unclear.
  - The physical store location (including main offices, store front, and warehouse) has sufficient locks, **CCTV surveillance**, and functioning fire detection and prevention systems.

</details>

---

## Control Categories

### Administrative/Managerial Controls
Administrative controls address the human aspect of cybersecurity. These include policies, procedures, and guidelines that manage data and define employee responsibilities. These policies may require technical or physical enforcement.

| Control Name             | Control Type  | Control Purpose                                                                 |
|--------------------------|---------------|---------------------------------------------------------------------------------|
| Least Privilege           | Preventative  | Reduces risk and the impact of malicious insiders or compromised accounts        |
| Disaster Recovery Plans   | Corrective    | Ensures business continuity after an incident                                   |
| Password Policies         | Preventative  | Reduces the likelihood of account compromise through attacks                    |
| Access Control Policies   | Preventative  | Enhances confidentiality by defining data access                                |
| Account Management        | Preventative  | Manages account lifecycle and reduces attack surfaces                           |
| Separation of Duties      | Preventative  | Reduces the risk and impact of malicious insiders                               |

### Technical Controls
Technical controls use technology to protect systems, networks, and data. These include firewalls, intrusion detection systems, encryption, and more.

| Control Name             | Control Type  | Control Purpose                                                                 |
|--------------------------|---------------|---------------------------------------------------------------------------------|
| Firewall                 | Preventative  | Filters unwanted or malicious traffic                                           |
| IDS/IPS                  | Detective     | Detects and prevents anomalous traffic based on rules                           |
| Encryption               | Deterrent     | Provides confidentiality to sensitive information                               |
| Backups                  | Corrective    | Restores systems after an event                                                 |
| Password Management      | Preventative  | Reduces password fatigue                                                        |
| Antivirus (AV) Software  | Corrective    | Detects and quarantines known threats                                           |

### Physical/Operational Controls
These controls manage physical access to assets like servers, networks, and other physical resources, including surveillance and locks.

| Control Name             | Control Type              | Control Purpose                                                                 |
|--------------------------|---------------------------|---------------------------------------------------------------------------------|
| Time-Controlled Safe      | Deterrent                 | Reduces attack surface from physical threats                                    |
| Adequate Lighting         | Deterrent                 | Deters threats by eliminating hiding spots                                      |
| CCTV                      | Preventative/Detective    | Acts as both a deterrent and a means of monitoring events                       |
| Locking Cabinets          | Preventative              | Prevents unauthorized access to network equipment                               |
| Signage                   | Deterrent                 | Deters attacks by making the chances of success seem lower                      |
| Fire Detection            | Detective/Preventative    | Detects fires and prevents physical asset damage                                |

### Conclusion
By auditing these control categories, we ensure the organization is equipped with proper defenses to secure its assets. Each control serves a vital role in protecting against unauthorized access, reducing threats, and maintaining business continuity.

---

# Botium Toys: Security Controls and Compliance Checklist

This summarizes the results of the security audit performed on Botium Toys' security controls and compliance with key frameworks, such as PCI DSS, GDPR, and SOC (Type 1, Type 2). This shows the current state of controls, compliance gaps, and recommendations for improvement.

## Security Controls Checklist

### Administrative Controls
| Control Name             | In Place?    |
|--------------------------|--------------|
| Least Privilege           | ❌ No        |
| Separation of Duties      | ❌ No        |

### Technical Controls
| Control Name             | In Place?    |
|--------------------------|--------------|
| Firewall                 | ✅ Yes       |
| Intrusion Detection System (IDS) | ❌ No  |
| Antivirus Software       | ✅ Yes       |
| Password Policies        | ❌ No        |
| Password Management System | ❌ No      |
| Encryption               | ❌ No        |
| Backups                  | ❌ No        |

### Physical Controls
| Control Name             | In Place?    |
|--------------------------|--------------|
| Locks (offices, storefront, warehouse) | ✅ Yes |
| Closed-circuit television (CCTV) | ✅ Yes  |
| Fire Detection/Prevention | ✅ Yes       |

## Compliance Checklist

### PCI DSS Compliance
| Compliance Best Practice                                      | In Place?    |
|---------------------------------------------------------------|--------------|
| Only authorized users have access to customers’ credit card information. | ❌ No |
| Credit card information is stored, processed, transmitted securely.       | ❌ No |
| Data encryption for credit card transaction touchpoints and data.         | ❌ No |
| Secure password management policies.                                       | ❌ No |

### GDPR Compliance
| Compliance Best Practice                                      | In Place?    |
|---------------------------------------------------------------|--------------|
| EU customers’ data is kept private/secured.                              | ✅ Yes |
| Breach notification plan within 72 hours.                                | ✅ Yes |
| Data properly classified and inventoried.                                | ❌ No  |
| Enforce privacy policies and documentation.                              | ✅ Yes |

### SOC (Type 1, Type 2) Compliance
| Compliance Best Practice                                      | In Place?    |
|---------------------------------------------------------------|--------------|
| User access policies are established.                                   | ❌ No  |
| Sensitive data (PII/SPII) is confidential/private.                       | ❌ No  |
| Data integrity is ensured (consistent, complete, accurate).              | ✅ Yes |
| Data availability is ensured for authorized users.                      | ✅ Yes |

## Recommendations

Based on the audit findings, the following controls and compliance practices need immediate attention to improve the security posture of Botium Toys:

- **Implement least privilege and separation of duties** to reduce unauthorized access and prevent internal threats.
- **Establish disaster recovery plans** and **regular data backups** to ensure business continuity.
- **Implement stronger password policies** and adopt a **centralized password management system**.
- **Deploy encryption** for sensitive customer data, particularly credit card information.
- **Install an Intrusion Detection System (IDS)** to detect and respond to anomalous network activity.
- **Enforce user access policies** to meet SOC compliance requirements.
- **Classify and inventory data** to enhance GDPR compliance.

By addressing these gaps, Botium Toys will significantly reduce its risk and better protect sensitive data.



