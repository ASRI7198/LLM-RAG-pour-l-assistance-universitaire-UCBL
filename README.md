# LLM-RAG pour l’assistance universitaire UCBL 🤖🎓

# InfoBot UCBL

<div align="center">
  <img src="img/Interface.png"">
  <br>
</div>

## Objective 🎯
**LLM-RAG pour l’assistance universitaire UCBL** is a chatbot powered by Large Language Models (LLM) using **Retrieval-Augmented Generation (RAG)** on university web pages. It is designed to assist students by providing accurate, up-to-date, and context-aware information about the Computer Science Department at Claude Bernard Lyon 1 University.  

The chatbot can:  
- answer academic queries 📝  
- support cover letter template creation ✍️  
- offer tailored certification recommendations from Coursera 🎓  

## Features ⚡
- **Question & Answering**: The chatbot can retrieve precise information about academic programs, research facilities, and opportunities at the university.  
- **Cover Letter Assistance**: The chatbot can suggest skills and experiences tailored to specific programs or roles.  
- **Certification Recommendations**: The chatbot can identify relevant certifications to enhance academic and professional profiles.  

## Technologies 🛠️
1. **LangChain**:  
   - Used for data loading, chunking, and efficient retrieval mechanisms.  
   - Documentation: [LangChain](https://www.langchain.com/docs)  
   
2. **Markdownify**:  
   - Converts HTML web pages into clean and structured Markdown format.  
   - Documentation: [Markdownify](https://pypi.org/project/markdownify/)  
   
3. **Sentence-Transformers (SBERT)**:  
   - Embedding model used to vectorize documents for semantic search.  
   - Documentation: [Sentence-Transformers](https://www.sbert.net/)  
   
4. **Chroma**:  
   - Vector database for fast and accurate retrieval of context-relevant data.  
   - Documentation: [Chroma](https://docs.trychroma.com/)  
   
5. **Llama 3.3**:  
   - Large Language Model used for question generation, context retrieval, and response generation.  
   - Documentation: [Llama Models](https://ai.meta.com/llama/)  

6. **Groq**:  
   - API used for accessing the Large Language Model (LLM).  
   - Documentation: [Groq](https://www.groq.com/)  
   
7. **Streamlit**:  
   - Framework used to build the application interface.  
   - Documentation: [Streamlit](https://docs.streamlit.io/)  

## Process & System Architecture 🏗️
1. **Data Collection**: Extracts information from the Computer Science Department's web pages and Coursera certifications.  
2. **Data Preprocessing**: Cleans, structures, and converts the data into Markdown format using Markdownify.  
3. **Data Chunking & Augmentation**: Splits data into manageable chunks and augments each chunk with questions summarizing its content.  
4. **Data Embedding & Storage**: Vectorizes the data using Sentence-Transformers and stores it in Chroma databases.  
5. **Query Handling**: Uses RAG to fetch relevant context for queries, enabling the chatbot to provide accurate and meaningful responses.  

![LLM-RAG UCBL System Architecture](img/Architecture_no_borders.jpg "LLM-RAG pour l’assistance universitaire UCBL")  

## Running the Application 🚀
1. **API Key**:  
   - You will need a Groq API key to access the LLM.  
2. **Install Requirements**:  
   - Open the `runApp.ipynb` file and install the dependencies.  
3. **Download Public IP**:  
```bash
!wget -q -O - ipv4.canhazip.com

