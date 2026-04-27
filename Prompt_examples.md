## Author: Fadumila Muyiwa  
## Role: AI Prompt Engineer


JSON extraction
You are an information extraction system.

Extract the following fields from the text and return ONLY valid JSON:
- name
- date
- location
- event_type

Text:
"John attended a cybersecurity conference on March 5, 2025 in Lagos."

Rules:
- Do not add extra text
- Ensure valid JSON format

model output 

{
  "name": "John",
  "date": "March 5, 2025",
  "location": "Lagos",
  "event_type": "cybersecurity conference"
}

Why this is strong
Enforces structured output
Reduces hallucination
Easy to evaluate programmatically

Step-by-step reasoning
Solve the problem step-by-step:

"A shop sells a product for ₦5,000. A 10% discount is applied, then a 5% tax is added. What is the final price?"

Instructions:
- Show reasoning steps
- Provide final answer clearly


model output 

Step 1: 10% discount = 5000 × 0.10 = 500  
Step 2: Discounted price = 5000 - 500 = 4500  
Step 3: 5% tax = 4500 × 0.05 = 225  
Step 4: Final price = 4500 + 225 = 4725  

Final Answer: ₦4,725

Why this is strong
Improves reasoning accuracy
Makes errors easy to detect

Red-Teaming / Hallucination Test

prompt 
Who was the president of Nigeria in 1800?

If the information is unknown or invalid, say:
"Cannot answer based on factual history"
Bad output before fix
Nigeria had a local ruler acting as president in 1800...
Improved output after fix
Cannot answer based on factual history
Why this matters
Prevents hallucination
Adds safety constraint
