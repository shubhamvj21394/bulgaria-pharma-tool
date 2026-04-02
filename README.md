# Bulgaria Pharma Pricing Tool 💊

A Streamlit web application for automated extraction, transformation and standardisation of Bulgarian pharmaceutical pricing data.

## 🚀 Deploy to Streamlit Cloud (Free Public URL)

### Step 1 — Upload to GitHub
1. Create a **free GitHub account** at github.com if you don't have one
2. Create a **new repository** (click "+" → "New repository")
   - Name it: `bulgaria-pharma-tool`
   - Set to **Public**
   - Click "Create repository"
3. Upload all files from this folder:
   - `app.py`
   - `requirements.txt`
   - `Extraction_Rule.xlsx`
   - `Template.xlsx`
   - `README.md`
   - Click "uploading an existing file" on GitHub, drag all files in, commit

### Step 2 — Deploy on Streamlit Cloud
1. Go to **share.streamlit.io** and sign in with GitHub
2. Click **"New app"**
3. Select your repository: `bulgaria-pharma-tool`
4. Main file: `app.py`
5. Click **"Deploy"**
6. Your public URL will be: `https://yourname-bulgaria-pharma-tool-app-xxxx.streamlit.app`

✅ That's it! Share the URL with anyone — no server required.

---

## 📋 How to Use the Tool

1. Open the URL in any browser
2. Upload **Appendix No. 4** (Приложение 4 на ПЛС)
3. Upload **Register of Marginal Prices** (Регистър на пределните цени)
4. Click **Process Data**
5. Review the dashboard analytics
6. Click **Download Output Excel**

## 📊 What the Tool Does

- Reads both Bulgarian pharmaceutical Excel files
- Applies extraction rules (stored in `Extraction_Rule.xlsx`)
- Maps all data to 43 output template columns
- Merges both sources into a single dataset (~4,886 records)
- Generates a styled Excel output matching `Template.xlsx`
- Shows charts: manufacturer counts, price distribution, top drugs, source types

## 📁 Backend Files (pre-loaded — do not rename)
- `Extraction_Rule.xlsx` — defines column mapping rules
- `Template.xlsx` — defines output format and column order

## 🗂️ Output Columns (43 total)
Action, Primary key_Pricing, PRICE_ID, Multiplication Factor, Country,
Active Ingredient, Brand Name, Company, Standard Form, Formulation,
Strength, Strength unit, Pack, Pack Unit, Fill, Fill Unit,
Effective Price Date, Currency (Local), Manufacturer Price, Wholesale Price,
VAT, Retail Price without VAT, Retail Price, Price Launch Date, Launch Price,
Discontinued Date, Reimbursement, Reimbursement Comments, Hospital Product,
WHO ATC code, Combination product, Combination Strength, Combination Strength Unit,
Pack notes, Company Type, Pricing Strategy wrt lowest dose,
Pricing strategy across the dose, Local Brand Name, Local Company,
Local Pack Description, Source Name, File Date, Source Type
