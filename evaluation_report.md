## Author: Fadumila Muyiwa  
## Role: AI Prompt Engineer

Title:.LLM Prompt Evaluation – Data Extraction Task
Objective:
Evaluate accuracy and consistency of structured JSON outputs.
 Test Setup
Task: Extract structured data
Models tested: GPT-style LLM
Prompts: Initial vs Refined

Before Improvement
Issues Found:
Invalid JSON format
Missing fields
Extra explanations outside JSON

Example Output 
{
  "name": "John"
}
This event happened recently.

Improvements Applied

Added strict instruction: “Return ONLY JSON”
Specified required fields
Removed ambiguity

After Improvement
Results:
 100% valid JSON
 All fields present
 No extra text

 Evaluation Metrics.    
 Metric.                Before.       After
Format Accuracy.        60%.           100%
Completeness.           70%.           100%
Instruction Adherence.  65%.           100%
