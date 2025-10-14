This dataset contains information collected for the study:

Loconte, R. & Kleinberg, B. (2025). Examining embedded lies through computational text analysis. Scientific Reports. DOI:10.1038/s41598-025-11327-w  

⸻

Columns

1. Participant Information
	•	Participant_id (string) – Unique identifier for each participant.
	•	Fluent_languages (string) – Self-reported languages spoken fluently.
	•	Age (integer) – Age in years.
	•	Sex (string) – Gender identity (e.g., Male, Female, Prefer not to say).
	•	Nationality (string) – Reported nationality.
	•	Language (string) – Native language.
	•	Student status (string: Yes/No) – Whether the participant is a student.
	•	Employment status (string) – Employment type (e.g., Full-time, Part-time).

⸻

2. Task Duration
	•	Duration_sec (integer) – Total duration of the experiment in seconds.
	•	Duration_min (float) – Same as above, converted to minutes.

⸻
3. Event selection 
	•	List_of_events (string) – Self-reported list of events that participants experienced within the past 24 months
	•	Event (string) – Experienced event that was randomly assigned to the participant
	•	Title_event (string) – Same as above, except for those who selected the option "None of them" and decided to go to an open-ended event and provided a title for it.


⸻

4. Memory-Related Event Variables
	•	Time_event (integer/categorical) – How long ago the selected autobiographical event happened (scale: <1 to 24 months).
	•	Recollection_event (integer, 1–5) – Frequency of thinking/talking about the event.
	•	Importance_event (integer, 1–5) – Subjective importance of the event.
	•	Accuracy_event (integer, 1–5) – How accurately the participant remembers the event.
	•	Valence_event (float, -1 to 1) – Emotional tone of the event (negative to positive).

⸻

5. Event description
	•	Task_order (categorical) – TL if participants wrote their statement first truthfully (T) and then deceptively (L); LT if they wrote the statement first deceptively (L) and then truthfully (T).
	•	True_event (string) – this is the full truthful statement about the selected event 
	•	True_event_tokens (string) – tokenized full truthful statement
	•	True_event_clean (string) – cleaned version of the full truthful statement; cleaning included punctuation and stopwords removal, and lemmatisation.
	•	True_event_num_words (integer) – number of words for the truthful statement
	•	False_event (string) – this is the deceptive statement with embedded lies about the selected event 
	•	False_event_tokens (string) – tokenized deceptive statement with embedded lies about the selected event 
	•	False_event_clean (string) – cleaned version of the deceptive statement; cleaning included punctuation and stopwords removal, and lemmatisation.
	•	False_event_num_words (integer) – number of words for the deceptive statement

⸻


6. Embedded Lies Variables
	•	Embedded_lies_*(string) – single words, phrases, or sentences that participants annotated as embedded lies in their deceptive statements
	•	*_deceptiveness (float, 1–5) – Perceived deceptiveness of the specific embedded lie (participant rating).
	•	*_centrality (float, 1–5) – Importance of the specific embedded lie for the overall narrative.
	•	*_source (categorical) – Origin of the specific embedded lie: past experience, others’ experience, imagination, media, or future plans.
	•	El_abs_num (integer) – Total number of embedded lies (from 1 to 20)
	•	merged_lies (string) - concatenated embedded lies texts 
	•	merged_lies_tokens (string) - tokenised embedded lies texts 
	•	merged_lies_clean (string) - cleaned embedded lies texts; cleaning included stopwords and punctuation removal, and lemmatisation.
	• 	EL_num_words (integer) – Total number of words used for embedded lies
	• 	EL_stand_num (float 0-1) - Ratio of embedded lie words to total words in the deceptive statement.
	• 	deceptiveness (float 1-5) - Average of the deceptiveness scores contained in the columns from 1_deceptiveness to 20_deceptiveness
	• 	centrality (float 1-5) - Average of the centrality scores contained in the columns from 1_centrality to 20_centrality 
	
* goes from 1 to 20

⸻


7. Additional Self-Reports
	•	Difficulty (integer, 1–5) – How difficult the participant found the task.
	•	Clarity (integer, 1–5) – Clarity of instructions.
	•	Motivation_truth (integer, 1–5) – Motivation to provide a convincing truthful statement.
	•	Motivation_lie (integer, 1–5) – Motivation to provide a convincing deceptive statement.

⸻

8. Lying Profile Questionnaire (raw scores)
	•	LIE_Frequency (float) – Self-reported frequency of lying.
	•	LIE_Ability (float) – Perceived ability to lie.
	•	LIE_Negativity (float) – Negative attitudes toward lying.
	•	LIE_Contextuality (float) – Positive/context-dependent attitudes toward lying.

⸻

9. Social Desirability (BIDR Scale)
	•	SDE (float) – Self-deceptive enhancement (unconscious positive bias).
	•	IM (float) – Impression management (conscious positive self-presentation).
	•	BIDR (float) – Overall BIDR score.

⸻

10. Lying Profile (adjusted for BIDR)
	•	LIE_Ability_adj (float) – Ability to lie (adjusted for social desirability).
	•	LIE_Contextuality_adj (float) – Contextual lying attitude (adjusted).
	•	LIE_Frequency_adj (float) – Frequency of lying (adjusted).
	•	LIE_Negativity_adj (float) – Negativity toward lying (adjusted).
	•	LIE_Profile (string: “Virtuous” / “Trickster”) – Cluster assignment of participant’s lying profile.

