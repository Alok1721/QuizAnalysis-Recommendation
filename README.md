This repo for Complete analysis of user details and it also recommand the topic that should focus on for 
1. analysing the data
2. preprocessing the data by removing the unnecessary columns
3. my major focus numerical data for analyse the user performance pattern/trends
4. plot various plot, through which user can analyse their performance throughout their quiz 
5. at last, this will suggest on which subject user should focus for better output
![Image](https://github.com/user-attachments/assets/4b503815-edc2-430e-bd5f-4c5d4438d09a)

![Image](https://github.com/user-attachments/assets/c29f0392-b4e0-4263-a227-7148d0840274)

## Brief Summary
<p>The recommendation process is based on analyzing quiz performance data and categorizing topics into different strength levels (Weak, Moderate, Strong) using statistical measures. Here's how it works:

Data Cleaning & Preparation:

The accuracy column (which may contain percentage symbols) is cleaned by converting it to a decimal format (e.g., 90% → 0.90).
Numerical columns (correct_answers, incorrect_answers, final_score, negative_score) are converted to numeric types, handling any invalid values gracefully.
Aggregation of Metrics:

The mean and standard deviation (std) are calculated for key performance indicators such as score, accuracy, and final score.
This aggregated data helps in understanding overall trends in performance across different quizzes.
Strength Classification:

Each quiz attempt is classified based on the mean and standard deviation of the score:
Weak (0): If the mean score is low (<50) or the standard deviation is high (>15), indicating inconsistency.
Moderate (1): If the mean score is between 50-80 or if the standard deviation is moderate (10-15), indicating average performance.
Strong (2): If the mean score is high (>80) and the standard deviation is low (<10), indicating consistent strong performance.
Grouping by Quiz ID:

The data is grouped by quiz_id to summarize the number of weak, moderate, and strong performances per quiz.
This helps in identifying which quizzes/topics need more focus and where the user excels.
Recommendations Based on Strength Levels:

Focus Areas: Quizzes with a higher count of Weak topics are suggested for improvement.
Reinforcement Areas: Quizzes with more Moderate topics can be suggested for revision.
Mastery Areas: Quizzes classified as Strong indicate proficiency and may not require further practice.</p>
## Setup
you have to run main.ipynb file , all important thing written on it. 
