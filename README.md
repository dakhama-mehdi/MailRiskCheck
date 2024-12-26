# MailRiskCheck

MailRiskCheck is a security audit project designed to test the effectiveness of email security systems.  
It focuses on evaluating how well anti-spam solutions and sandboxing can detect and handle potentially malicious email attachments.  

## Purpose

The main goal of this project is to test the resilience of email security solutions by sending a BMP image containing a compiled file and a tool like Mimikatz.  
The test aims to check if the system can detect these hidden threats and block them effectively.

| **Feature**                  | **Description**                                                                                     |
|------------------------------|-----------------------------------------------------------------------------------------------------|
| **Testing Email Security**   | The project simulates the delivery of malicious content via email.                                   |
| **Bypassing Anti-Spam**      | Tests whether spam filters can detect potentially harmful files disguised as harmless image files.  |
| **Sandbox Evaluation**       | Assesses the ability of sandbox environments to handle and analyze malicious payloads.              |
| **Governance Testing**       | Tests the governance of allowed file types and the internal email security policies for accepting attachments like BMP files. |
| **Usage Testing**            | Verifies the usage of the image in real-world email scenarios and how it is handled by security systems. |


## Usage

- **Sending via External Mail**: Send the BMP image as an attachment from an external email to a test internal email inbox.
- **SOC and EDR Reactivity**: After receiving the email, attempt to save and open the image to test the reactivity of your Security Operations Center (SOC) and Endpoint Detection and Response (EDR) solutions.
- **VirusTotal Check**: Verify the image on VirusTotal to see if any engines detect the hidden payload.

