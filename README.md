README

This repository contains code used in the research for automating Performance Status (PS) annotation in oncology patient records using Llama-3. The files are organized into categories based on the specific tasks they address. Below is a step-by-step guide on how to use the files in the correct order.

1. Generalizing Dataset Identifiers
1a. Create_Global_Dataset_with_Unique_Identifiers.ipynb
   - Purpose: Generalizes dataset identifiers and creates a global dataset with unique note identifiers.

2. Sampling Patients for Validation and Test Sets
2a. Initial_Patient_Sampling_for_Validation_and_Test_Sets.ipynb
   - Purpose: Samples patients for the validation and test sets based on the initial dataset.

2b. First_Round_Annotation_Insights.ipynb
   - Purpose: Provides insights from the first round of annotations to refine the sampling process.

2c. Second_Round_Patient_Sampling_with_Refined_Criteria.ipynb
   - Purpose: Conducts the second round of patient sampling after refining the criteria based on insights from the first round.

3. Extracting and Censoring Pre-Annotated PS-Scores
3a. Extract_PreAnnotated_PS_Scores_with_RegEx.ipynb
   - Purpose: Uses Regular Expressions to extract pre-annotated PS scores from the dataset.

3b. Censor_PS_Scores_in_Dataset.ipynb
   - Purpose: Censors explicit mentions of PS scores in the dataset to avoid bias during annotation.

4. Converting INCEpTION Annotations to Annotated Dataset
4a. Convert_INCEpTION_Annotations_to_CSV.ipynb
   - Purpose: Converts annotations from INCEpTION into a CSV format.

4b. Process_CSV_Annotations_to_Annotated_Dataset.ipynb
   - Purpose: Processes the CSV annotations to create a structured annotated dataset.

4c. Review_and_Confirm_Positive_Labels_from_INCEpTION.ipynb
   - Purpose: Manually reviews and confirms positive labels from the INCEpTION annotations.

5. Creating Folds for Validation and Test Sets
5a. Split_Annotated_Dataset_into_Sentence_Rows.ipynb
   - Purpose: Splits the annotated dataset into individual sentence rows (with note-number) for further processing.

5b. Create_Stratifed_Folds_for_Validation_and_Test_Sets.ipynb
   - Purpose: Creates stratified folds for the validation and test sets.

6. Selecting Examples for One- and Few-Shot Learning
6a. Select_ACSESS_Examples_for_Each_Fold.ipynb
   - Purpose: Selects examples for each fold using the ACSESS method for one- and few-shot learning.

6b. Randomly_Select_Examples_for_Each_Fold.ipynb
   - Purpose: Randomly selects examples for each fold as a baseline comparison.

6c. Select_ACSESS_Examples_from_Validation_for_Test_Set.ipynb
   - Purpose: Selects examples from the validation set using ACSESS for application on the test set.

7. Running Llama on Examples and Data
7a. Run_Llama_on_Validation_Set_with_ACSESS_Random_Manual_Examples.ipynb
   - Purpose: Runs the Llama model on the validation set using examples selected by ACSESS, random, and manual example selection.

7b. Run_Llama_on_Test_Set_with_ACSESS_Examples.ipynb
   - Purpose: Runs the Llama model on the test set using examples selected by ACSESS.

8. Evaluation Metrics
8a. Evaluate_Binary_Classification_Task.ipynb
   - Purpose: Evaluates the binary classification task's performance metrics (e.g., Precision, Recall, F1-score).

8b. Evaluate_Regression_Task_Performance.ipynb
   - Purpose: Evaluates the regression task's performance metrics (e.g., MAE, MSE, RMSE).
