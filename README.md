# Resume Analyzer and LinkedIn Job Scraper

**Project Link**
https://resume-analyzer-using-generative-ai.streamlit.app/

## Introduction

Resume Analyzer AI" leverages the power of LLM and OpenAI as an advanced Streamlit application, specializing in thorough resume analysis. It excels at summarizing the resume, evaluating strengths, identifying weaknesses, and offering personalized improvement suggestions, while also recommending the perfect job titles. Additionally, it seamlessly employs Selenium to extract vital LinkedIn data, encompassing company names, job titles, locations, job URLs, and detailed job descriptions. In essence, Resume Analyzer AI simplifies the job-seeking journey by equipping users with comprehensive insights to elevate their career opportunities.

**Resume Used**

View Resume [here](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/Richie%20Singh%20Resume.pdf).

**Summary Visualization**

![Summary](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/summary.png "Summary Visualization")

**Strengths**

![Strength](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/strength.png "Strengths Analysis")

**Weaknesses**

![Weakness](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/weakness.png "Weaknesses Analysis")

**Identified Job Titles**

![Job Titles](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/job%20titles.png "Identified Job Titles")

**Find Linkedin Jobs for that Position**

![LinkedIn Jobs](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/linkedin_jobs.png "LinkedIn Jobs Visualization")

**List of Linkedin Jobs**

![List LinkedIn Jobs](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/images/list_linkedin_jobs.png "List of LinkedIn Jobs")

**Key Technologies and Skills**
- Python
- Numpy
- Pandas
- Streamlit
- LLM
- LangChain
- OpenAI
- Selenium


**Installation**

To run this project, you need to install the following packages:

```python
pip install numpy
pip install pandas
pip install streamlit
pip install streamlit_option_menu
pip install streamlit_extras
pip install PyPDF2
pip install langchain
pip install openai
pip install tiktoken
pip install faiss-cpu
pip install selenium
```
**Architecture**

![Project_Architecture](https://github.com/richiectr360/resume-analyzer-using-generative-ai-llm/blob/main/Workflow%20Architecture.png)


**Usage**

To use this project, follow these steps:

1. Install the required packages: ```pip install -r requirements.txt```
2. Run the Streamlit app: ```streamlit run app.py```
3. Access the app in your browser at ```http://localhost:8501```


**Features**

**Easy User Experience:**
- Resume Analyzer AI makes it easy for users. You can upload your resume and enter your OpenAI API key without any hassle. The application is designed to be user-friendly so that anyone can use its powerful resume analysis features.
- It also uses the PyPDF2 library to quickly extract text from your uploaded resume, which is the first step in doing a thorough analysis.

**Smart Text Analysis with Langchain:**
- What makes it special is how it analyzes text. It uses a smart method called the Langchain library to break long sections of text from resumes into smaller chunks, making them more meaningful.
- This clever technique improves the accuracy of the resume analysis, and it gives users practical advice on how to enhance their job prospects.

**Enhanced OpenAI Integration with FAISS:**
- Seamlessly connecting to OpenAI services, the application establishes a secure connection using your OpenAI API key. This integration forms the basis for robust interactions, facilitating advanced analysis and efficient information retrieval.
- It uses the FAISS(Facebook AI Similarity Search) library to convert both the text chunks and query text data into numerical vectors, simplifying the analysis process and enabling the retrieval of pertinent information.

**Intelligent Chunk Selection and LLM:**
- Utilizing similarity search, Resume Analyzer AI compares the query and chunks, enabling the selection of the top 'K' most similar chunks based on their similarity scores.
- Simultaneously, the application creates an OpenAI object, particularly an LLM (Large Language Model), using the ChatGPT 3.5 Turbo model and your OpenAI API key.

**Robust Question-Answering Pipeline:**
- This integration establishes a robust question-answering (QA) pipeline, making use of the load_qa_chain function, which encompasses multiple components, including the language model.
- The QA chain efficiently handles lists of input documents (docs) and a list of questions (chunks), with the response variable capturing the results, such as answers to the questions derived from the content within the input documents.

**Comprehensive Resume Analysis:**
- **Summary:** Resume Analyzer AI provides a quick, comprehensive overview of resumes, emphasizing qualifications, key experience, skills, projects, and achievements. Users can swiftly grasp profiles, enhancing review efficiency and insight.
- **Strength:** Effortlessly conducting a comprehensive resume review, it analyzes qualifications, experience, and accomplishments. It subsequently highlights strengths, providing job seekers with a competitive edge.
- **Weakness:** AI conducts thorough analysis to pinpoint weaknesses and offers tailored solutions for transforming them into strengths, empowering job seekers.
- **Suggestion:** AI provides personalized job title recommendations that align closely with the user's qualifications and resume content, facilitating an optimized job search experience.


