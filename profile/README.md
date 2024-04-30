# ChatGPT Firewall - Your pal to cost-efficiently and securely chat with arbitrarily large documents

Welcome to ChatGPT Firewall, a versatile prompt firewall designed specifically for ChatGPT and related LLM models. This tool enables you to engage in secure and cost-effective conversations while safeguarding sensitive data and files:

- prompt ChatGPT with extensive documents or a large number of documents, overcoming the limitations of GPT-3's context capacity. For instance, it enables tokenization of materials such as books, electronic patient records, or contracts.
- opt in or out pseudonymizing prompts, ensuring privacy by sanitizing personal information such as names, email addresses, and street names. If uncomfortable with potentially sensitive content within prompts, automated suggestions can be manually post-edited for added security and peace of mind.
 
## Getting started

- **Try it**: [https://chatgpt.enclaive.io/](https://chatgpt.enclaive.io/)
- **Build it**: [https://github.com/ChatGPTfirewall/ChatGPTfirewall](https://github.com/ChatGPTfirewall/ChatGPTfirewall)
- **Project Page**: [https://chatgptfirewall.github.io/ChatGPTfirewall/](https://chatgptfirewall.github.io/ChatGPTfirewall/)
- **Documentation**: [https://chatgptfirewall.gitbook.io/chatgptfirewall/](https://chatgptfirewall.gitbook.io/chatgptfirewall/)


## Features

- **Conversational Data Interaction**: Users can chat with their data by uploading files and asking questions in natural language.
- **File Upload Support**: Manual file uploads.
- **Vector Database Integration**: Utilizes Qdrant for efficient similarity searches on text data.
- **Editable Responses**: Adjust the number of sentences returned from searches.
- **Customizable Prompts**: Customize the prompts sent to ChatGPT for tailored answers.
- **Authentication**: Secure user login with Auth0.
- **File Management**: Easily manage your uploaded files.
- **Demo Mode**: Explore the application's capabilities with preloaded files in demo mode.
- **Multilingual**: The application supports both German and English languages.
- **Rooms**: Create different rooms for different contexts.

## Releases 

v0.1:

- **Reduced prompt length**: Rather than tokenizing the entire document, chatGPTfw employs a [retrieval augmented generation (RAG)](https://qdrant.tech/articles/what-is-rag-in-ai/)  system, utilizing the [qdrant][https://qdrant.tech/] vector database. This process condenses the prompt down to the three most probable responses.
  
v0.2:
- **File-Based Chatting**: Enables asking questions about uploaded file contents. Currently supported formats: PDF, TXT

v0.3:
- **Confidential Cloud Environment**: Deployment scripts to run in a confidential compute environemt. Learn  [more](https://enclaive.io/)
- **Pseudonymize Data**: Masks sensitive information in prompt to ensure privacy (e.g. name, location, email address) before sending to chatGPT

v0.4:
- **DE/EN language support**: Chat with docs in DE and EN

v0.5:
- **Demo mode/use cases**: Chat with files containing an excerpt of sections from book or a series of court rulings

## Contribute

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**. If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Acknowledgments

This project greatly celebrates all contributions from the open source community. Big shout out to

- [qdrant](https://qdrant.tech/) vector database
