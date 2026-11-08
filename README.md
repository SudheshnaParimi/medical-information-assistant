# medical-information-assistant
A healthcare AI agent built using Azure AI Foundry and GPT-4.1 to provide accurate, safe, and patient-friendly medical information with knowledge base integration and guardrails.


🏥 Medical Information Assistant using Azure AI Foundry

1. Experiment Overview

This experiment focuses on building a Medical Information Assistant using Microsoft Azure AI Foundry and the GPT-4.1 model.

The objective is to develop an AI agent that provides accurate, clear, and patient-friendly medical information while following healthcare safety guidelines.

The assistant is designed to answer general medical questions without providing personal diagnoses or treatment recommendations.

2. Experiment Environment

The experiment is performed in Microsoft Azure AI Foundry.

Component	Configuration
Platform	Azure AI Foundry
AI Model	GPT-4.1
Agent Name	Medical Information Assistant
Temperature	0.3
Knowledge Base	Basic Medical Terminology
Guardrail	Microsoft.DefaultV2
Testing	Azure AI Foundry Playground

3. Implementation

The following steps are performed:

1. Agent Creation: Created a Medical Information Assistant using GPT-4.1.
2. AI Instructions: Configured the agent to provide general medical information with an empathetic tone and a mandatory medical disclaimer.
3. Temperature Setting: Set the temperature to 0.3 for more consistent responses.
4. Knowledge Base Integration: Added the Basic Medical Terminology document to support medical explanations.
5. Guardrail Configuration: Reviewed the inherited Microsoft.DefaultV2 guardrail.
6. Testing: Defined five medical queries to evaluate the assistant’s responses.

4. Guardrail Settings

The agent inherits the Microsoft.DefaultV2 guardrail from its deployed model. No separate agent-level guardrail is assigned.

Risks With Controls

Risk	Controls
Jailbreak	1
Content Safety	4
Protected Materials	2

Risks Without Controls

* Indirect Prompt Injections
* Sensitive Data Leakage
* Task Drift

These risks require additional safeguards before production deployment.

5. Testing Scenarios

The agent is tested using five medical information queries.

Scenario	Test Query	Expected Result
1	What is diabetes?	Explain diabetes in simple language.
2	Explain MRI procedure.	Describe MRI and how it works.
3	What are antibiotics?	Explain antibiotics and their purpose.
4	Define hypertension.	Explain high blood pressure.
5	How does vaccination work?	Explain how vaccines support immunity.

Evaluation Criteria

Each response is evaluated for:

* Medical accuracy
* Clear and empathetic communication
* Inclusion of the medical disclaimer
* Appropriate use of the knowledge base

6. Conclusion

This experiment demonstrates how to create a healthcare AI agent using Azure AI Foundry and GPT-4.1.

The assistant is configured with safety instructions, a medical knowledge base, and an inherited guardrail to support responsible medical information delivery.

The five testing scenarios provide a foundation for evaluating response accuracy, clarity, and safety.

Further improvements can include stronger security controls, additional medical resources, and more extensive testing before real-world deployment.

⸻

Note: This project is intended for educational purposes and does not replace professional medical advice.
