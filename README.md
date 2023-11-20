# NICE-TalentDiscovery

Cybersecurity Talent discovery project as per 'NIST NICE Framework' using NLP and Machine Learning techniques.

I acquired the NICE Framework KSAs data from the official website (snapshot attached) and cleaned and organized the dataset into CSV format. To emulate a talent community, I collected technical resumes from Kaggle that include current job roles and comprehensive resume text. The dataset is available at https://www.kaggle.com/datasets/gauravduttakiit/resume-dataset/.

I created a Python script to match employees with the most appropriate roles based on the content of their resumes and the corresponding Knowledge, Skills, and Abilities (KSA) descriptions in the dataset. The employee resumes and KSA descriptions undergo preprocessing, which includes tokenization, conversion to lowercase, and removal of stop words. The TF-IDF vectorization method is then applied to convert the textual data into numerical representations. Subsequently, cosine similarity is calculated between the vectorized employee resumes and the aggregated KSA descriptions grouped by Role ID. The role with the highest cosine similarity is designated as the most suitable role for each employee.
