# Resume Analyzer

This repository contains the source code for an automated resume sorting and analysis tool. It uses Natural Language Processing (NLP) and machine learning techniques to parse, match, select, and rank resumes from an extensive pool, all predicted on the basis of the job description.

## Project Description

In a world where countless job seekers are applying for positions, businesses often get overwhelmed by the sheer volume of resumes. Each resume possesses a distinct structure and content, deviating from any standardized format. This project aims to automate the process of sifting through these individualistic documents to pinpoint the ideal candidate for a specific job.

The tool is designed to mimic how recruiters review each resume in their database, seeking those that seamlessly align with the job description. The selected resumes then go through a ranking process, where relevance to the job description becomes the defining metric. Finally, key candidate details such as their name, contact information, and email address are accessed for further steps of the application process.

## How it Works

1. The script reads all resumes and job descriptions from specified directories.
2. Text information is extracted from these documents.
3. Preprocessing is performed to clean up the text data.
4. TF-IDF vectorization is applied to convert textual data into numerical form.
5. Feature reduction is carried out using Truncated Singular Value Decomposition (SVD).
6. Cosine similarity between resumes and job descriptions is calculated.
7. Candidate's name, email ID, phone number, skills, experience years etc., are extracted from each resume.
8. Resumes are sorted based on their relevance score for each job role.
9. Word clouds are generated for visual representation of key skills required in each role.

## Dependencies

- pandas
- google-colab
- pdfminer3
- nltk
- sklearn
- en_core_web_sm
- matplotlib
- wordcloud
- mammoth
- locationtagger

## Usage

Replace the directory paths for resumes and job descriptions in the script, and run the script. The script will output a sorted list of candidates for each job role based on their relevance score.

Please note that this is a basic implementation and might not work perfectly for all types of resumes and job descriptions. You may need to tweak the code according to your specific use case.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
