# Skill-Test
Problem: 

Develop a Stenography/Typing Test evaluation system that accurately assesses the performance of candidates by comparing their transcripts to a master file. The system should adhere to the evaluation guidelines specified, including the classification of mistakes, calculation of error percentages, and handling of alternate word forms. 

Input: 

Master File: The reference transcript against which candidate transcripts will be evaluated.
Candidate Files: The transcripts submitted by stenography candidates for evaluation.
Dictionary: A list of permitted replaced words, allowing for minor spelling variations.

Output: 

Evaluated File: For each candidate transcript, an updated file indicating the identified mistakes and their corresponding types (full or half).
Error Percentage Report: A summary report for each candidate, including the total number of mistakes, percentage of errors, and a breakdown of full and half mistakes.
Specific Requirements:
Process multiple candidate transcripts efficiently.
Handle nested data structures, such as lists of words and nested dictionaries, to accommodate the structure of transcripts and dictionaries. 
Incorporate error handling to gracefully manage invalid inputs or unexpected data structures. 

Error Classification and Calculation:

Full Mistakes:

Omission of words or figures: Count each omitted word or figure as a full mistake. 
Substitution of wrong words or figures: Count each substitution as a full mistake. 
Addition of extra words or figures: Count each extra word or figure as a full mistake. 

Half Mistakes:

Wrong spelling: Count each misspelled word as half a mistake. 
Singular-plural noun errors: Count each singular-plural error as half a mistake. 
Small letters at sentence beginnings: Count each small letter error as half a mistake.

Error Percentage Calculation:

Calculate the total number of mistakes (full mistakes + half mistakes/2). 
Divide the total number of mistakes by the number of words in the master passage. 
Multiply the result by 100 to get the percentage of errors. 
Round the percentage to two decimal places. 

Handling Alternate Word Forms: 
Use a dictionary to check if a candidate's spelling is an acceptable alternative. 
If the candidate's spelling is in the dictionary, do not count it as an error. 
