
AR-ASAG Dataset The ARabic Dataset for Automatic Short Answer Grading Evaluation   



                        Questions/Student Answers with Grades
                          ==========================
                            
                                    Version 1.0
                                   
                                November 25th, 2019

                           Leila OUAHRANI*, Djamal BENNOUAR**

                                 Bouira University 
                                       Algeria 

                                *l_ouahrani@univ-blida.dz  
                                **djamal.bennouar@univ-bouira.dz 

  

CONTENTS
1. Introduction
2. Data Set
2.a. Data Annotation
2.b. Folder Structure
3. Feedback
4. Citation Info
5. Acknowledgments




=======================
1. Introduction

This README v1.0 (November, 2019) for the Arabic Automatic Short Answer Grading Dataset
This is a dataset to explore and research the Automatic Short Answer Grading (ASAG) field. 
 

=======================
2. Data Set

=====
2.a. Data Annotation

Our dataset consists of reported evaluations relate to answers submitted for three different exams submitted 
to three classes of students. The exams were conducted under natural conditions of evaluation. 
Each test consists of 16 short answer questions (a total of 48 questions). 
For each question, a model answer is proposed. 
Students submitted answers to these questions.  
The number of answers obtained is different from one question to another. 
The dataset includes a total of 2133 pairs (Model Answer, student answer). 
the Dataset encompasses 5 types of questions:
•	"عرف ": 		Define?
•	"إشرح":			Explain?
•	"ما النتائج المترتبة على": 	What consequences?
•	"علل": 			Justify?
•	"ما الفرق": 		What is the difference

AR-ASAG Dataset is available in different versions: TXT, XML, XML-MOODLE and Database (.DB).   
The .DB format allows to make the necessary exports according to specific analysis needs.  
The XML-MOODLE format is used on Moodle e-learning Platforms
 
Please see here for more information about : Moodle-Short Answer Question Type : 
https://docs.moodle.org/37/en/Short-Answer_question_type

For each pair, two grades (Mark1 and Mark2 ) are associated with a manual Average Gold Score
Both manual grades are available in the dataset.
Inter-Annotators Agreement:  - (Pearson Correlation: r=0.8384) 
			     - (Root Mean Square Error : RMSE=0.8381). 

For privacy reasons, no student identifiers are used in this Dataset.
=====
2.b. Folder Structure

*AR-ASAG DataSet
	This folder contains Four sub_folders for TXT, XML, XML-MOODLE and Database (.DB) Versions
	The name of file is representative of its content. 
	We use the term "Mark" to specify "Grade"

     Sub-Folders :

	TXT-Version folder : 
		Files : (Model Answers List - 48).txt
			(Questions List - 48).txt
			(Student Answers List).txt
			(Number Of Answers  For Each Question For the 48 Questions).txt
			(Questions- Model Answers - Student Answers - Average Gold).txt
			(Questions- Model Answers - Student Answers - Grade1- Grade2-  Average Gold).txt
			(AR-ASAG-480).txt : A sampling  sub dataset of 480 couples (48*10) of (model answer, student answer) including                                               all questions. It's obtained after a randomized split and then the first ten answers are                                                 selected for each question.
	XML-Version Folder :
		Files : (Type - Questions).xml
			(Questions-Model Answers).xml
			(Questions- Students Answers - Grade1 - Grade2 - Average Gold).xml
			(Questions- Students Answers - Average Gold).xml

	XML-Moodle-Version Folder:
		File : (MoodleXML- Questions - Student  Answers - Average Gold).xml
	 

=======================
3. Feedback

For further questions or inquiries about this dataset, you can contact:
l_ouahrani@univ-blida.dz  
 


=======================
4. Citation Info 

@InProceedings{ouahrani-bennouar:2020:LREC,
author = {Ouahrani, Leila and Bennouar, Djamal},
title = {AR-ASAG An ARabic Dataset for Automatic Short Answer Grading Evaluation},
booktitle = {Proceedings of The 12th Language Resources and Evaluation Conference},
month = {May},
year = {2020},
address = {Marseille, France},
publisher = {European Language Resources Association},
pages = {2634--2643},
abstract = {Automatic short answer grading is a significant problem in E-assessment. Several
models have been proposed to deal with it. Evaluation and comparison of such solutions need the
availability of Datasets with manual examples. In this paper, we introduce AR-ASAG, an Arabic
Dataset for automatic short answer grading. The Dataset contains 2133 pairs of (Model Answer,
Student Answer) in several versions (txt, xml, Moodle xml and .db). We explore then an
unsupervised corpus based approach for automatic grading adapted to the Arabic Language. We use
COALS (Correlated Occurrence Analogue to Lexical Semantic) algorithm to create semantic space for
word distribution. The summation vector model is combined to term weighting and common words to
achieve similarity between a teacher model answer and a student answer. The approach is
particularly suitable for languages with scarce resources such as Arabic language where robust
specific resources are not yet available. A set of experiments were conducted to analyze the
effect of domain specificity, semantic space dimension and stemming techniques on the
effectiveness of the grading model. The proposed approach gives promising results for Arabic
language. The reported results may serve as baseline for future research work evaluation},
url = {https://www.aclweb.org/anthology/2020.lrec-1.321}
}
=======================
5. Acknowledgments

This work is supported by the project C00L07UN100120180002 of the Ministry of 
Higher Education and Scientific Research in Algeria. 
Authors are grateful to Faiza OUKINA and Imene AMARSETTI for their technical help.  

