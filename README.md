# **Market Basket Analysis (Aisle-Level)**



## ***Project Overview***

This notebook-driven project performs a Market Basket Analysis at the aisle/category level using the Instacart “Online Grocery Basket Analysis” dataset. By mining association rules, it uncovers which store aisles tend to co-occur in customer orders—insights that can inform store layout, cross-merchandising, and targeted promotions.



## ***Dataset***

Source: https://www.kaggle.com/datasets/yasserh/instacart-online-grocery-basket-analysis-dataset  

Expected files (place in `Dataset/` folder):

&nbsp; -orders.csv  

&nbsp; -order\_products\_\_prior.csv  

&nbsp; -products.csv

&nbsp; -aisles.csv



## ***Folder Structure***

market-basket/

├── .gitignore

├── LICENSE

├── README.md

├── requirements.txt

├── 01\_Notebook.ipynb

├── venv/                   # Virtual environment (ignored via .gitignore)

└── Dataset/                # Raw data files (ignored via .gitignore)

## 

## ***Environment Setup***

#### <i>1. Clone the repository </i> 

&nbsp;  git clone https://github.com/<your-username>/market-basket-analysis.git

&nbsp;  cd market-basket-analysis

&nbsp;  

#### *2. Create \& activate a Python 3.8+ virtual environment*

&nbsp;  python -m venv venv -> # Windows

&nbsp;  .\\venv\\Scripts\\activate -> # macOS/Linux

&nbsp;  

#### *3. Install dependencies*  

&nbsp;  pip install -r requirements.txt

&nbsp;  



## ***Usage***

#### *1. Place your CSV files in the `Dataset/` folder.*  

#### *2. Launch JupyterLab*  

&nbsp;  jupyter lab

&nbsp;    

#### *3. Open `01\_Notebook.ipynb` and run all cells in order (1 through 7) to:*

&nbsp;  - Load and clean data  

&nbsp;  - Merge aisle metadata  

&nbsp;  - Build a one-hot “order × aisle” basket  

&nbsp;  - Sample 100,000 orders for performance  

&nbsp;  - Run Apriori and generate association rules  

&nbsp;  - Visualize the top 10 aisle-level rules



## ***Key Findings***

\- The strongest association in our 100k-order sample was:

&nbsp; {baking goods} → {sweet snacks} (Lift ≈ 2.5)

\- Other high-lift aisle pairs reveal complementary sections that can be co-promoted.



### ***Dependencies***

\- pandas  

\- mlxtend  

\- matplotlib  

\- jupyterlab  

\*(See `requirements.txt` for exact version pins.)



### ***License***

This project is released under the MIT License. See `LICENSE` for details.



