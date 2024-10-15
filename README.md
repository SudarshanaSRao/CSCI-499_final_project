# FAQ Generator

Final LLM Project for USC CSCI-499 (Language Models in Natural Language Processing)

#### [Medium blog](https://medium.com/@sudarshanasrao/faq-generation-using-large-language-models-88746c9381a6)

## Overview
![fine-tuning drawio](https://github.com/SudarshanaSRao/CSCI-499_final_project/assets/87690830/17d0ee7e-906e-49b3-995b-5e2191f161c6)

### Background

Large Language Models (LLMs) have become a household word nowadays. LLMs have compelling applications, and this project explores the effectiveness of Large Language Models (LLMs) in generating Frequently Asked Questions (FAQs) solely from graduate school's admission requirements for Master of Science in Computer Science. T5-large, BART-large, LLaMA-2, and LLaMA-3 performances were investigated, employing a tailored dataset to examine their capabilities in an FAQ generation context. Each model was fine-tuned with data specifically oriented towards eliciting admission-related inquiries, aligning closely with the real-world information needs of prospective students.

### Objective

The objective of the project is to develop an advanced natural language processing system capable of autonomously generating high-quality FAQs for websites based on their content. This involves fine-tuning several state-of-the-art language models including Llama-3 8b, Llama-2 7b, Mistral 7b, T5, and BART, integrating QLoRA PEFT for enhanced FAQ quality, and creating a comprehensive dataset by scraping and storing admission requirements for the top 150 US universities' MS in CS programs. The goal is to achieve a significant improvement in FAQ accuracy and relevance, aiming for a 10% increase compared to a baseline T5 transformer model.

![text_summary_gpt drawio](https://github.com/SudarshanaSRao/CSCI-499_final_project/assets/87690830/7c423744-57f7-45e2-8392-09750b4c917f)

### Dataset

A list of the top 150 US universities for the CS program based on USNews rankings was compiled. The university names and website URLs were stored in a CSV file. Using the BeautifulSoup library, web scraping on each URL was performed, extracting admission requirements and existing FAQs. This collected data was then structured into a JSON file for compatibility with the language model training process. The dataset was split into training, validation, and testing sets as per the ratio 80\%:10\%:10\%.


