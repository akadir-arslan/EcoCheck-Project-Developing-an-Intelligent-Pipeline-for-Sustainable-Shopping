# EcoCheck Project: Developing an Intelligent System for Sustainable Shopping

**Project Overview:**
The EcoCheck project focused on building an intelligent system for the EcoCheck app, designed to assist consumers in making sustainable shopping choices. By providing detailed information about food products—such as regionality, sustainability, and manufacturing conditions—EcoCheck simplifies sustainable shopping for consumers. Much of the required data is not readily available in public databases, so the system was developed to automate the collection, categorization, and enhancement of product data from popular retailers, ensuring users have access to accurate and comprehensive product details.

**Key Tasks and Components:**

1. **Web Scraping:**
  - We as a team developed and enhanced web scraping programs to collect product data from various retailers, including Aldi Nord, Aldi Süd, Kaufland, Edeka24, Netto, Rossmann, and AlNatura.
  - Extracted data included product names, brands, prices, offers, sales, descriptions, ingredients, and more.
  - Solutions were implemented to address the challenges of dynamically generated websites and the ethical concerns of web scraping, such as using APIs (e.g., DM’s API) and affiliate services (e.g., Awin for Rewe 
    data) for more efficient data collection.

2. **Handling Missing Ingredient Data:**
  - A script was created to manage missing ingredient data by using the Serp API to search for product information on Google. The script retrieved the top five search results, extracted HTML content, and utilized 
    a Large Language Model (LLM) (GPT) to extract the necessary ingredient data from the gathered content.

3. **Product Categorization:**
  - Various approaches were explored to categorize products as vegan, vegetarian, and non-vegetarian. Initially, the team experimented with zero-shot learning and image recognition techniques, such as using the 
    Scale-Invariant Feature Transform (SIFT) algorithm to analyze packaging images. However, these methods did not yield satisfactory results.
  - The team then integrated OpenAI’s GPT model for product categorization by feeding it product names, descriptions, nutrients, and ingredient data. This approach led to significant improvements in 
    categorization accuracy and overall system performance.

**Project Results:**
The combination of web scraping, Serp API, and GPT integration enabled EcoCheck to create a more comprehensive and reliable product database. The project’s intelligent system (the pipeline) automates the process of collecting and categorizing product data from multiple retailers, enhancing the EcoCheck app’s ability to provide users with accurate and detailed information.

**Note:** Due to the privacy policy of EcoCheck, and the company's restrictions on sharing the database, code, and background information with third parties, I am unable to provide the code or other related documents in this repository.
