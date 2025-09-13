# VELO Chatbot Demographic Recommender  

## 📌 Overview  
This project develops a **Python-based chatbot** and **synthetic dataset generator** for **Velo Pakistan**.  
The chatbot collects structured demographic and consumer preference data via a decision-tree survey.  
The resulting dataset helps optimize flavour/strength assortments for small retailers and identify under-realized flavours for future trials.  

---

## 🎯 Objectives  
- **Store-Level Prioritization** → Recommend the best flavour/strength mix for each region and retailer type.  
- **Identify Under-Realized Flavours** → Detect flavours attractive to new users but underperforming among existing ones.  
- **Consumer Insights** → Build scalable demographic and preference datasets for product development and marketing.  

---

## 🛠️ Features  
- Decision-tree chatbot flow (age, gender, region, urban/rural, occupation, nicotine use, flavour preferences).  
- Synthetic dataset generation with **demographic multipliers** (urban vs rural, region, gender, age groups).  
- Weighted probability sampling for **flavour and strength selection**.  
- Output: structured dictionaries and CSV datasets ready for analysis.  

---

## 📂 Repository Structure  
velo-pk-chatbot-demographic-recommender/
│── notebooks/ # Jupyter notebooks (chatbot + dataset code)
│── data/ # Mock datasets (CSV)
│── docs/ # Project documentation (Word, PDF)
│── slides/ # Presentation slides (PPTX)
│── README.md # Project overview (this file)


---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Mlaf27/velo-pk-chatbot-demographic-recommender.git
   cd velo-pk-chatbot-demographic-recommender
2. Open the Jupyter notebook:
jupyter notebook notebooks/"chat bot model & mock dataset code.ipynb"
3. Run the cells to:
-Launch the chatbot demo.
-Generate synthetic consumer preference data.

## 📊 Dataset Generation Process

- Assign demographics (region, metro/rural, gender, age, occupation).
- Apply baseline probabilities for flavour categories (Spice, Mint & Menthol, Fruit) and strengths (Low, Medium, High).
- Adjust probabilities using demographic multipliers (e.g., urban → coffee flavours, rural → spearmint).
- Weighted random sampling → Select category, strength, and 3 unique flavours.
- Output dataset for analysis.

## ⚠️ Limitations
- Granularity → Only 4 regions + metro/rural considered; neighbourhood-level variations not captured.
- Response Bias → Survey on velo.com.pk may overrepresent existing Velo users.
- Large Files → Some presentation files exceed 50 MB (consider Git LFS if needed).

## 📈 Future Extensions
- Collect emails for CRM & marketing campaigns.
- Capture city- and neighbourhood-level preferences.
- Allow free-text feedback + AI clustering to detect emerging flavour trends.
- Integrate sentiment analysis for strength satisfaction.
- Deploy chatbot via WhatsApp/SMS for wider reach.

## 👥 Authors
Matthieu Lafont
Feroz Obaid Khan
Henry Wolcott
Okerein Emmanuel Ebipade
