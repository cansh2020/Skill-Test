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

a) Every omission of a word or figure. In case a group of words are omitted, as many mistakes as the actual number of omitted words will be counted. 
b) Every substitution of a wrong word or figure. If a figure is written correctly either in numeral or words both will be acceptable and will not be counted a mistake. The number of mistakes will be equal to the number of dictated word(s) not written by the candidate plus the number of wrongly substituted word(s).
c) Every addition of a word or figure or symbol not occurring in the dictated passage.
d) For repetition of word, e.g. ‘I shall shall be grateful…..
e) For every incomplete word(s).
f) All left-over word(s) of the passage.
g) Candidates are required to type the actual words as dictated. Abbreviations used for expanded words will be treated as full mistakes, and vice-versa.
h) If a candidate types words or lines of the passage in all Capital letters, it will be counted full mistakes. 

Half Mistakes:

a) Wrong spelling.
b) Using singular for plural noun and vice versa.
c) Omission of every Full Stop at the end of the sentence, or use of Full Stop at wrong place of the sentence will be treated as half mistake.
d) Use of small letter at the beginning of the sentence.
e) Non-capitalisation of Proper Noun (s) (name of a person, place, office, etc.), for example, Shyam, Parliament House, Bihar, Ministry of Home Affairs, StafSelection Commission, etc. 

Error Percentage Calculation:

Calculate the total number of mistakes (full mistakes + half mistakes/2). 
Divide the total number of mistakes by the number of words in the master passage. 
Multiply the result by 100 to get the percentage of errors. 
Round the percentage to two decimal places. 

Handling Alternate Word Forms: 
Use a dictionary to check if a candidate's spelling is an acceptable alternative. 
If the candidate's spelling is in the dictionary, do not count it as an error. 
