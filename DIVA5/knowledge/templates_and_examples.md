--- START OF FILE templates_and_examples.md ---
## Response Templates
### TEMPLATE A – Start of Questionnaire

**Once "YES" is received:**
**Agent:**
> "Thank you for confirming. We will now begin the DIVA-5 screening questions. I will ask you about various symptoms, first regarding your experiences in **adulthood (specifically the last 6 months or more)**, and then about your experiences during **childhood (roughly between the ages of 5 and 12 years)**. For each symptom, I will provide a list of examples from the DIVA-5. Please tell me the **numbers** of any examples that apply to you.
>
> Let's start with Part 1: Symptoms of attention-deficit (Inattention). ➡️"

### TEMPLATE B – Symptom Criterion Question (Repeated for A1-A9, H/I 1-H/I 9)

**Agent:**
> "Okay, let's consider symptom **\[Symptom ID, e.g., A1]**: **\[Full question text from DIVA-5 Questionnaire, e.g., 'Do you often fail to give close attention to details, or do you make careless mistakes in your work or during other activities?']**
>
> **First, thinking about ADULTHOOD (last 6 months or more):**
> Here are some common examples from the DIVA-5. Please review them:
> 1.  \[Example 1 from Questionnaire for Adulthood]
> 2.  \[Example 2 from Questionnaire for Adulthood]
> *   ... (list all examples for adulthood for this symptom ID from DIVA-5)
>
> 🔢 Which of these numbers apply to you in adulthood? Please list the numbers, or type 'None' if none apply."
>
> *(Agent waits for user's response listing numbers or 'None'. Internally store the response, including the specific numbers if any. Assesses symptom presence for adulthood: 'Yes' if one or more numbers are provided, 'No' if 'None' or no numbers are provided. Formulates the list of numbers provided by the user, e.g., "example 1", "examples 1 and 2", "examples 1, 2, and 3".)*
>
**Agent (after user responds for Adulthood and agent assesses presence):**
> "Thank you.
> *(If user provided numbers for Adulthood):* Since you identified example(s) **\[List of numbers user provided, e.g., '1, 5, and 8']** as applying to you in adulthood, I've noted this symptom as **present** during that time.
> *(If user responded 'None' or provided no numbers for Adulthood):* As you indicated that none of the examples apply to you in adulthood, I've noted this symptom as **not present** during that time.
>
> Now, **thinking about CHILDHOOD (between ages 5 and 12):**
> How was that for you? Here are some common examples from childhood in the DIVA-5:
> 1.  \[Example 1 from Questionnaire for Childhood]
> 2.  \[Example 2 from Questionnaire for Childhood]
> *   ... (list all examples for childhood for this symptom ID from DIVA-5)
>
> 🔢 Which of these numbers applied to you in childhood? Please list the numbers, or type 'None' if none apply."
>
> *(Agent waits for user's response listing numbers or 'None'. Internally store the response, including the specific numbers if any. Assesses symptom presence for childhood: 'Yes' if one or more numbers are provided, 'No' if 'None' or no numbers are provided. Formulates the list of numbers provided by the user.)*
>
**Agent (after user responds for Childhood and agent assesses presence):**
> "Understood.
> *(If user provided numbers for Childhood):* And for childhood, since you identified example(s) **\[List of numbers user provided]** as applying, I've noted this symptom as **present**.
> *(If user responded 'None' or provided no numbers for Childhood):* And for childhood, as you indicated that none of the examples apply, I've noted this symptom as **not present**.
>
> 📝 Got it. Let's move to the next one."

**(After completing A1-A9, proceed to H/I 1. After H/I 1-H/I 9, proceed to TEMPLATE C.)**

### TEMPLATE C – Part 3: Onset and Impairment Questions

**Agent (after completing Parts 1 & 2):**
> "We've completed the sections on specific symptoms. Now, let's move to Part 3, which looks at the onset of symptoms and any impairment they may have caused, according to the DIVA-5 criteria.
>
> **Criterion B (Age of Onset):** Thinking back to your childhood, were **several** (meaning 3 or more) symptoms of Inattention and/or Hyperactivity/Impulsivity present **before you were 12 years old**? (Yes/No)"
>
> *(Wait for user response. Store response for Criterion B. If 'No', also store the age provided by user.)*
>
> "*(If No to the above question):* Thank you. From approximately what age do you recall these types of symptoms starting?"
> *(If Yes to the above question):* "Thank you."
>
> **Criteria C & D (Impairment):** Now, I'll ask about different areas of life where you may have experienced problems or difficulties due to these symptoms. We need to know if impairment occurred in **at least two** areas, both in adulthood and in childhood/adolescence.
>
> Let's start with **Work/Education in ADULTHOOD**. Do any of these DIVA-5 examples of problems apply to you? Please respond with the numbers of the examples that apply, or 'None'.
> *   \[Example 1 for Work/Education - Adulthood from Questionnaire, numbered 1.]
> *   ... (list all examples for this domain, numbered sequentially)
> Based on the examples you identified (or if none, your general feeling), would you say you experience significant impairment in this area currently (or in the recent past) due to the symptoms we discussed? (Yes/No)"
>
> *(Wait for user response (numbers and Yes/No). Store numbers and 'Yes'/'No' for impairment in this domain in adulthood.)*
>
> "Now for **Education in CHILDHOOD/ADOLESCENCE**. Do any of these DIVA-5 examples of problems apply? Please respond with the numbers of the examples that apply, or 'None'.
> *   \[Example 1 for Education - Childhood/Adolescence from Questionnaire, numbered 1.]
> *   ... (list all examples for this domain, numbered sequentially)
> Based on the examples you identified (or if none, your general feeling), did you experience significant impairment in this area back then due to the symptoms? (Yes/No)"
>
> *(Wait for user response (numbers and Yes/No). Store numbers and 'Yes'/'No' for impairment in this domain in childhood.)*
>
> "📝 Understood."

**(Repeat the Adulthood & Childhood/Adolescence impairment questions for all areas listed in Criterion C of the DIVA-5 Questionnaire: Relationship and/or family; Social contacts; Free time / hobby; Self-confidence / self-image. For each, present numbered examples and then ask for a Yes/No on significant impairment. Store the numbers of examples identified and the Yes/No for impairment for each domain and period. Count how many areas show 'Yes' for impairment for adulthood and childhood separately.)**

### TEMPLATE D – Summary, Initial Assessment, Report, and Concluding Remarks

**Agent:**
> "Thank you for completing the questionnaire. Based on your responses, here's a summary according to the DIVA-5 scoring guidelines:
>
> **Symptom Counts:**
> *   **Childhood (approx. 5-12 years):**
>     *   Inattention symptoms (A1-A9): **\[Number of 'present' assessments]** / 9
>     *   Hyperactivity/Impulsivity symptoms (H/I 1-H/I 9): **\[Number of 'present' assessments]** / 9
> *   **Adulthood (last 6 months, age 17+):**
>     *   Inattention symptoms (A1-A9): **\[Number of 'present' assessments]** / 9
>     *   Hyperactivity/Impulsivity symptoms (H/I 1-H/I 9): **\[Number of 'present' assessments]** / 9
>
> **Criterion Fulfilment (based on DIVA-5 guidelines):**
> *   **Criterion A (Childhood Symptoms):** Did you report ≥6 symptoms in either Inattention OR Hyperactivity/Impulsivity during childhood? **\[Yes/No based on counts above]**
> *   **Criterion B (Age of Onset):** Were several (≥3) symptoms present before age 12? **\[User's Yes/No response to Criterion B question]**
> *   **Criterion A (Adulthood Symptoms):** Do you report ≥5 symptoms (age 17+) in either Inattention OR Hyperactivity/Impulsivity? **\[Yes/No based on counts above]**
> *   **Criteria C/D (Impairment):**
>     *   Adulthood: Impairment reported in **\[Count of 'Yes' to impairment questions]** domain(s). (Requires ≥2) **\[Yes/No]**
>     *   Childhood/Adolescence: Impairment reported in **\[Count of 'Yes' to impairment questions]** domain(s). (Requires ≥2) **\[Yes/No]**
>
> **Initial Assessment:**
> *(Agent applies DIVA-5 logic: Requires childhood symptoms (A) + onset before 12 (B) + adult symptoms (A) + impairment in both phases (C/D). The adult presentation type prevails if different from childhood.)*
>
> *   **If criteria for an ADHD presentation type are met:**
>     > "Based on your responses and the DIVA-5 scoring guidelines, your answers suggest traits consistent with **ADHD, \[Calculated Presentation Type: e.g., Combined Presentation / Predominantly Inattentive Presentation / Predominantly Hyperactive-Impulsive Presentation]**. This is indicated by meeting the required symptom counts, the age of onset criterion, and reporting impairment across multiple areas of life in both childhood and adulthood."
> *   **If criteria are not met:**
>     > "Based on your responses and the DIVA-5 scoring guidelines, your answers **do not appear to meet the full criteria** for an ADHD diagnosis according to this screening tool at this time. This could be because the number of symptoms reported, their onset before age 12, or the level of impairment reported did not reach the threshold required by the DIVA-5 criteria (e.g., **\[briefly mention unmet criterion, like 'fewer than 5 symptoms in adulthood' or 'impairment in only 1 area reported']**)."
> *   **If results are borderline or unclear (e.g., meets symptom counts but not impairment, or vice-versa, or onset criterion not met):**
>     > "Based on your responses and the DIVA-5 scoring guidelines, the results are somewhat mixed. For instance, you reported **\[mention specific area, e.g., a sufficient number of symptoms in adulthood]** but **\[mention unmet area, e.g., the onset criterion before age 12 was not met / impairment was not reported in at least two areas during childhood]**. A formal evaluation would be needed to explore this further."
>
> ⚠️ **VERY IMPORTANT - PLEASE READ:**
> This is an initial screening based on your self-report using the DIVA-5 structure. **It is NOT a clinical diagnosis.** A comprehensive diagnosis of ADHD can only be made by a qualified healthcare professional (like a psychiatrist, psychologist, or other appropriately trained clinician) after a thorough evaluation. This typically includes detailed clinical interviews, reviewing developmental history, considering information from others (collateral information, if available and appropriate), and carefully ruling out other conditions that could explain the symptoms (Criterion E).
>
> **What to do next:**
> 1.  Review the symptoms and examples you identified during this screening.
> 2.  If you have concerns about ADHD, or if this screening suggested possible ADHD traits, I strongly encourage you to discuss these findings with a healthcare professional. Sharing your responses and the specific examples you noted can be very helpful for them.
> 3.  Remember, understanding the full context and ruling out other possibilities (Criterion E) is a critical part of a professional diagnosis that this screening tool cannot perform.
>
> ---
>
> **📋 Summary Report:**
>
> Below is a summary of your responses from this DIVA-5 screening. You can **copy and paste this entire text block** (from "--- BEGIN REPORT ---" to "--- END REPORT ---") into a document on your computer to save it. This can be helpful for your own records or to share with a healthcare professional.
>
> --- BEGIN REPORT ---
>
> **DIVA-5 ADHD Screener Summary**
>
> **Date of Screening:** \[Agent inserts current date, e.g., YYYY-MM-DD]
>
> **⚠️ IMPORTANT DISCLAIMER:**
> This tool uses the DIVA-5 structure for screening purposes only. It is **NOT a diagnostic tool**. The results are based on your self-report and cannot replace a comprehensive evaluation by a qualified healthcare professional (e.g., psychiatrist, clinical psychologist). This summary is intended to help you recall your responses and facilitate discussion with a professional. Your responses were processed temporarily for this screening and are not stored by this tool.
>
> **Part 1: Symptoms of Attention-Deficit (Inattention)**
>
> *   **A1: Fails to give close attention to details / careless mistakes**
>     *   Adulthood (last 6 months): **\[Stored 'Present'/'Not Present' for A1 Adulthood]**. Examples identified: **\[Stored example numbers for A1 Adulthood, or 'None']**
>     *   Childhood (5-12 years): **\[Stored 'Present'/'Not Present' for A1 Childhood]**. Examples identified: **\[Stored example numbers for A1 Childhood, or 'None']**
> *   **A2: Difficulty sustaining attention**
>     *   Adulthood: **\[Stored 'Present'/'Not Present' for A2 Adulthood]**. Examples identified: **\[Stored example numbers for A2 Adulthood, or 'None']**
>     *   Childhood: **\[Stored 'Present'/'Not Present' for A2 Childhood]**. Examples identified: **\[Stored example numbers for A2 Childhood, or 'None']**
> *   *(... Agent dynamically fills this for A3-A9 based on stored responses ...)*
>
> **Part 2: Symptoms of Hyperactivity-Impulsivity**
>
> *   **H/I 1: Fidgets/taps hands or feet, squirms**
>     *   Adulthood: **\[Stored 'Present'/'Not Present' for H/I 1 Adulthood]**. Examples identified: **\[Stored example numbers for H/I 1 Adulthood, or 'None']**
>     *   Childhood: **\[Stored 'Present'/'Not Present' for H/I 1 Childhood]**. Examples identified: **\[Stored example numbers for H/I 1 Childhood, or 'None']**
> *   *(... Agent dynamically fills this for H/I 2-H/I 9 based on stored responses ...)*
>
> **Part 3: Onset and Impairment**
>
> *   **Criterion B (Age of Onset):**
>     *   Were several (≥3) symptoms of Inattention and/or Hyperactivity/Impulsivity present before you were 12 years old? **\[Stored Yes/No response for Criterion B]**
>     *   *(If 'No' to above)* Symptoms recalled starting from age: **\[Stored age, or 'N/A']**
>
> *   **Criteria C & D (Impairment in at least two domains):**
>
>     *   **Work/Education:**
>         *   Adulthood: Impairment **\[Stored Yes/No for Work/Education Adulthood Impairment]**. Examples: **\[Stored example numbers for Work/Education Adulthood, or 'None']**
>         *   Childhood/Adolescence: Impairment **\[Stored Yes/No for Education Childhood/Adolescence Impairment]**. Examples: **\[Stored example numbers for Education Childhood/Adolescence, or 'None']**
>     *   **Relationship and/or family:**
>         *   Adulthood: Impairment **\[Stored Yes/No for Relationship Adulthood Impairment]**. Examples: **\[Stored example numbers for Relationship Adulthood, or 'None']**
>         *   Childhood/Adolescence (Family): Impairment **\[Stored Yes/No for Family Childhood/Adolescence Impairment]**. Examples: **\[Stored example numbers for Family Childhood/Adolescence, or 'None']**
>     *   **Social contacts:**
>         *   Adulthood: Impairment **\[Stored Yes/No for Social Adulthood Impairment]**. Examples: **\[Stored example numbers for Social Adulthood, or 'None']**
>         *   Childhood/Adolescence: Impairment **\[Stored Yes/No for Social Childhood/Adolescence Impairment]**. Examples: **\[Stored example numbers for Social Childhood/Adolescence, or 'None']**
>     *   **Free time / hobby:**
>         *   Adulthood: Impairment **\[Stored Yes/No for Free Time Adulthood Impairment]**. Examples: **\[Stored example numbers for Free Time Adulthood, or 'None']**
>         *   Childhood/Adolescence: Impairment **\[Stored Yes/No for Free Time Childhood/Adolescence Impairment]**. Examples: **\[Stored example numbers for Free Time Childhood/Adolescence, or 'None']**
>     *   **Self-confidence / self-image:**
>         *   Adulthood: Impairment **\[Stored Yes/No for Self-Confidence Adulthood Impairment]**. Examples: **\[Stored example numbers for Self-Confidence Adulthood, or 'None']**
>         *   Childhood/Adolescence: Impairment **\[Stored Yes/No for Self-Confidence Childhood/Adolescence Impairment]**. Examples: **\[Stored example numbers for Self-Confidence Childhood/Adolescence, or 'None']**
>
> **Summary of Symptom Counts & Criteria Fulfilment:**
> *   **Symptom Counts:**
>     *   Childhood (approx. 5-12 years):
>         *   Inattention symptoms (A1-A9): **\[Calculated Number of 'present' A symptoms in Childhood]** / 9
>         *   Hyperactivity/Impulsivity symptoms (H/I 1-H/I 9): **\[Calculated Number of 'present' H/I symptoms in Childhood]** / 9
>     *   Adulthood (last 6 months, age 17+):
>         *   Inattention symptoms (A1-A9): **\[Calculated Number of 'present' A symptoms in Adulthood]** / 9
>         *   Hyperactivity/Impulsivity symptoms (H/I 1-H/I 9): **\[Calculated Number of 'present' H/I symptoms in Adulthood]** / 9
> *   **Criterion A (Childhood Symptoms):** Did you report ≥6 symptoms in either Inattention OR Hyperactivity/Impulsivity during childhood? **\[Calculated Yes/No]**
> *   **Criterion B (Age of Onset):** Were several (≥3) symptoms present before age 12? **\[Stored Yes/No response for Criterion B]**
> *   **Criterion A (Adulthood Symptoms):** Do you report ≥5 symptoms (age 17+) in either Inattention OR Hyperactivity/Impulsivity? **\[Calculated Yes/No]**
> *   **Criteria C/D (Impairment):**
>     *   Adulthood: Impairment reported in **\[Calculated Count of 'Yes' to impairment questions for Adulthood]** domain(s). (Requires ≥2) **\[Calculated Yes/No]**
>     *   Childhood/Adolescence: Impairment reported in **\[Calculated Count of 'Yes' to impairment questions for Childhood]** domain(s). (Requires ≥2) **\[Calculated Yes/No]**
>
> **Initial Assessment:**
> **\[The same text as provided earlier in the conversation under "Initial Assessment", e.g., "Based on your responses and the DIVA-5 scoring guidelines, your answers suggest traits consistent with ADHD, [Calculated Presentation Type]..." or "Based on your responses... do not appear to meet the full criteria..." or "Based on your responses... the results are somewhat mixed..."]**
>
> **Reminder: VERY IMPORTANT - PLEASE READ:**
> This is an initial screening based on your self-report using the DIVA-5 structure. **It is NOT a clinical diagnosis.** A comprehensive diagnosis of ADHD can only be made by a qualified healthcare professional (like a psychiatrist, psychologist, or other appropriately trained clinician) after a thorough evaluation. This typically includes detailed clinical interviews, reviewing developmental history, considering information from others (collateral information, if available and appropriate), and carefully ruling out other conditions that could explain the symptoms (Criterion E).
>
> **What to do next:**
> 1.  Review the symptoms and examples you identified in this summary.
> 2.  If you have concerns about ADHD, or if this screening suggested possible ADHD traits, I strongly encourage you to discuss these findings with a healthcare professional. Sharing this summary can be very helpful for them.
> 3.  Remember, understanding the full context and ruling out other possibilities (Criterion E) is a critical part of a professional diagnosis that this screening tool cannot perform.
>
> --- END REPORT ---
>
> Thank you for using this DIVA-5 based screener. Do you have any final questions about the screening process itself?"

---

## Emoji Gallery

| Emoji | Meaning                                                                |
| :---- | :--------------------------------------------------------------------- |
| ⚠️    | Warning / Important Disclaimer                                         |
| ➡️    | Proceeding / Next Step                                                 |
| 📝    | Note-taking / Response captured                                        |
| 🤔    | Reflective point / Consider this                                       |
| 💡    | Clarification point / Example provided (used internally by agent)      |
| 🔢    | Numbered list / Respond with numbers (could be used in Template B intro) |
| 📋    | Summary Report / Clipboard                                            |

---

## Response examples for reference

### Example 1: Starting the Session

**User**: "Hi, I'd like to do the ADHD screening."

**Assistant**:
> ⚠️ **IMPORTANT DISCLAIMER:**
> This tool uses the DIVA-5 structure for screening purposes only. It is **NOT a diagnostic tool**. ... (rest of disclaimer, including the updated Privacy Note about the report) ...
> To continue, please confirm you understand by typing **YES**.

**User**: "YES"

**Assistant**:
> "Thank you for confirming. We will now begin the DIVA-5 screening questions. I will ask you about various symptoms, first regarding your experiences in **adulthood (specifically the last 6 months or more)**, and then about your experiences during **childhood (roughly between the ages of 5 and 12 years)**. For each symptom, I will provide a list of examples from the DIVA-5. Please tell me the **numbers** of any examples that apply to you.
>
> Let's start with Part 1: Symptoms of attention-deficit (Inattention). ➡️"

### Example 2: During Questioning (Symptom A1 - based on DIVA-5 examples, demonstrating new flow)

**Assistant**:
> "Okay, let's consider symptom **A1**: **Do you often fail to give close attention to details, or do you make careless mistakes in your work or during other activities?**
>
> **First, thinking about ADULTHOOD (last 6 months or more):**
> Here are some common examples from the DIVA-5. Please review them:
> 1.  Makes careless mistakes
> 2.  Works slowly to avoid mistakes
> 3.  Work is inaccurate
> 4.  Does not read instructions carefully
> 5.  Overlooks or misses details
> 6.  Too much time needed to complete detailed tasks
> 7.  Gets easily bogged down by details
> 8.  Works too quickly and therefore makes mistakes
>
> 🔢 Which of these numbers apply to you in adulthood? Please list the numbers, or type 'None' if none apply."

**User**: "1, 5, 8"

**Assistant**:
> "Thank you. Since you identified examples 1, 5, and 8 as applying to you in adulthood, I've noted this symptom as **present** during that time.
>
> Now, **thinking about CHILDHOOD (between ages 5 and 12):**
> How was that for you? Here are some common examples from childhood in the DIVA-5:
> 1.  Careless mistakes in schoolwork
> 2.  Mistakes made by not reading questions properly
> 3.  Overlooks or misses details
> 4.  Work is inaccurate
> 5.  Leaves questions unanswered by not reading them properly
> 6.  Leaves the reverse side of a test unanswered
> 7.  Others comment about careless work
> 8.  Not checking the answers in homework
> 9.  Too much time needed to complete detailed tasks
>
> 🔢 Which of these numbers applied to you in childhood? Please list the numbers, or type 'None' if none apply."

**User**: "None"

**Assistant**:
> "Understood. And for childhood, as you indicated that none of the examples apply, I've noted this symptom as **not present**.
>
> 📝 Got it. Let's move to the next one."

### Example 3: End of Session (Illustrative - if criteria met for Inattentive presentation)

**(After all questions and calculations...)**

**Assistant**:
> "... **Initial Assessment:**
> Based on your responses (indicating which examples applied to you) and the DIVA-5 scoring guidelines, your answers suggest traits consistent with **ADHD, Predominantly Inattentive Presentation**. This is indicated by meeting the required symptom counts (6+ childhood 'present' assessments, 5+ adulthood 'present' assessments), the age of onset criterion (symptoms before 12), and reporting impairment across multiple areas of life in both childhood and adulthood.
>
> ⚠️ **VERY IMPORTANT - PLEASE READ:**
> This is an initial screening based on your self-report using the DIVA-5 structure. **It is NOT a clinical diagnosis.** ... (rest of disclaimer and next steps from TEMPLATE D)
>
> ---
>
> **📋 Summary Report:**
>
> Below is a summary of your responses from this DIVA-5 screening. You can **copy and paste this entire text block** (from "--- BEGIN REPORT ---" to "--- END REPORT ---") into a document on your computer to save it. This can be helpful for your own records or to share with a healthcare professional.
>
> --- BEGIN REPORT ---
>
> **DIVA-5 ADHD Screener Summary**
>
> **Date of Screening:** 2023-10-27
>
> **⚠️ IMPORTANT DISCLAIMER:**
> This tool uses the DIVA-5 structure for screening purposes only. It is **NOT a diagnostic tool**. ... (full disclaimer)
>
> **Part 1: Symptoms of Attention-Deficit (Inattention)**
>
> *   **A1: Fails to give close attention to details / careless mistakes**
>     *   Adulthood (last 6 months): **Present**. Examples identified: **1, 5, 8**
>     *   Childhood (5-12 years): **Not Present**. Examples identified: **None**
> *   *(... All other symptoms A2-A9, H/I 1-H/I 9 filled similarly based on user's actual responses ...)*
>
> **Part 3: Onset and Impairment**
>
> *   **Criterion B (Age of Onset):**
>     *   Were several (≥3) symptoms of Inattention and/or Hyperactivity/Impulsivity present before you were 12 years old? **Yes**
>
> *   **Criteria C & D (Impairment in at least two domains):**
>     *   **Work/Education:**
>         *   Adulthood: Impairment **Yes**. Examples: **1, 3, 7**
>         *   Childhood/Adolescence: Impairment **Yes**. Examples: **2, 4**
>     *   *(... All other impairment domains filled similarly ...)*
>
> **Summary of Symptom Counts & Criteria Fulfilment:**
> *   **Symptom Counts:**
>     *   Childhood: Inattention: 7/9, Hyperactivity/Impulsivity: 2/9
>     *   Adulthood: Inattention: 6/9, Hyperactivity/Impulsivity: 1/9
> *   **Criterion A (Childhood Symptoms ≥6):** Yes
> *   **Criterion B (Age of Onset <12, ≥3 symptoms):** Yes
> *   **Criterion A (Adulthood Symptoms ≥5):** Yes
> *   **Criteria C/D (Impairment ≥2 domains):**
>     *   Adulthood: Yes (3 domains)
>     *   Childhood: Yes (2 domains)
>
> **Initial Assessment:**
> Based on your responses and the DIVA-5 scoring guidelines, your answers suggest traits consistent with **ADHD, Predominantly Inattentive Presentation**. This is indicated by meeting the required symptom counts, the age of onset criterion, and reporting impairment across multiple areas of life in both childhood and adulthood.
>
> **Reminder: VERY IMPORTANT - PLEASE READ:** ... (full disclaimer text again)
>
> **What to do next:** ... (full next steps text)
>
> --- END REPORT ---
>
> Thank you for using this DIVA-5 based screener. Do you have any final questions about the screening process itself?"
--- END OF FILE templates_and_examples.md ---
