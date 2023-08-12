# Orgpedia - Information Extraction and Presentation for Public Good

[Orgpedia Foundation](https://www.orgpedia.in) is a Section 8 (non-profit) company based in Pune, India. Orgpedia intends to make it easy for people to understand the workings of government organizations; this is for both - people outside the organization as well as those inside the organization.

To achieve this broad goal, Orgpedia is focusing on solving two technology problems
   1. Build information extraction technology for extracting information from government orders.
   2. Present the information in a way that is easy to consume for even a common man.

## Orgpedia Projects
1. **Chat friendly extraction of Maharashtra Government Orders**: Orgpedia has converted last five years of Maharashtra Government orders (GRs) that are in marathi PDFs, to English and Marathi text files. They are in a format that is friendly for chat LLMs to consume. The pipeline does table structure extraction, translation and paragraph extraction. There are about 50,000+ orders in the repository and the data is available at https://github.com/orgpedia/mahGRs. The repository is updated weekly. 
\
\
On this data there is a simple chatbot that answers specific questions [video](https://www.youtube.com/watch?v=6e-jsZsTMDE), the chatbot uses OpenAI's apis. 
\
There is also a website where weekly summaries are published. The summaries are generated based on district and department and annotated with additional information like, funds allocated, category of the order. The goal is to provide rich annotations so that users can sign up for information that is relevant for them. https://mahsummary.orgpedia.in/

2. **Deep Extraction on Government Orders**: The idea is to convert a government order into a JSON object so that it can be added to a database and queries can be run on the database. I have been focussing on Government Orders that relate to posting and transfers of government officers. The goal here is to extract the information and build an org chart for that department. This was a very hard problem and could only make very little headway.
\
\
Currently we have only released the work for Indian Cabinet Ministers data. The site (https://www.orgpedia.in/prime.html) contains the cabinet information and the hierarchy for last 75 years, starting with the first cabinet, and country's first order to the date. 
\
The first order can be seen at  https://www.orgpedia.in/en/order-1_Upload_2027.pdf.html. Code/data at https://github.com/orgpedia/cabsec/. This site is available in 22 Indian languages and English.

3. **Chat friendly extraction of Gazette Data (WIP)**: We are currently processing Gazette data from Maharashtra and Karnataka, both these datasets are predominantly in Marathi and Kannada, respectively. The goal is to process the gazette data and split it in smaller relevant documents so that they can be easily consumed by a specialized chatbot. 

## Help needed for Orgpedia:

Orgpedia in near term wants to focus on two goals 
1) Do deep extraction on the order and gazette data and 
2) Offer a chat interface in native Indian language for a specific department/domain.

To achieve both these goals Orgpedia wants to build a specialized Indian Language model specifically for government data and for these two use cases. Furthermore, the hope is that the specialized model will perform reasonably well and at a much smaller size, making it afforadable to run for all. To achieve this goal, it will require converting large amounts of government data in Indian languages to text files and further computing resources for building the model.
I need help on both these fronts

  1) Cloud credits for using the OCR API.
  2) Computing Credits for building the specialized language model.

  *All the data and and source code is in open source (MIT license) and available on Orgpedia's GitHub repository https://github.com/orgpedia.*



