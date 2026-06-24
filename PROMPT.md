You must convert the text file I will provide into a CSV compatible with my “Quiz Trainer” website.

The website accepts ONLY this CSV format:

source;question;options;correct;explanation

Mandatory rules:
1. Use semicolon as the column separator: ;
2. Use exactly these columns, in this exact order:
   source;question;options;correct;explanation
3. Always wrap every field in double quotes.
4. If a field contains double quotes, escape them by doubling them.
   Example:
   "text with ""quotes"""
5. In the options field, separate all answer choices using:
   ||
   Example:
   "Answer A||Answer B||Answer C||Answer D"
6. In the correct field, write the exact text of the correct answer.
7. If a question has multiple correct answers, separate them using:
   ||
   Example:
   "Answer A||Answer C"
8. The correct value must exactly match one or more options listed in the options field.
9. Do not use letters such as A, B, C, D as correct answers unless the options themselves are literally A, B, C, D.
10. Create clear, unambiguous questions based only on the provided text.
11. Do not invent information that is not present in the text.
12. Each question must have at least 3 options, preferably 4.
13. Wrong options must be plausible but clearly false according to the text.
14. The explanation must briefly explain why the correct answer is correct.
15. In the source field, write a short name for the document, topic, chapter, or section.
16. If the text is divided into sections, use the section title as the source.
17. If the text does not contain enough reliable information, generate only the questions that can be made accurately.
18. Output ONLY the final CSV.
19. Do not use markdown.
20. Do not add comments before or after the CSV.
21. Do not use code blocks.
22. Do not add any extra text.

Goal:
Generate useful study questions, not shallow or obvious ones. Prioritize:
- important definitions
- key concepts
- differences between similar concepts
- causes and effects
- sequences or procedural steps
- formulas, rules, or conditions
- common mistakes
- details that could appear in an exam

Number of questions:
Generate as many good questions as possible, while avoiding useless repetition.

Before generating the CSV, reason internally about which concepts are actually worth testing. Do not show your reasoning. Output only the final CSV.

Required final format:

source;question;options;correct;explanation
"Source";"Question?";"Option 1||Option 2||Option 3||Option 4";"Correct option";"Brief explanation."

Here is the text to convert:

[PASTE THE TEXT HERE]