# 🌍 Climate Displacement Modeling  
## Environment Setup & Notebook Execution Guide

This guide explains how to correctly set up and run the Jupyter Notebook for this project on **Windows** and **macOS** using a clean Python virtual environment.
Our aggregated and final dataset we use to train the models is `processed_dataset.csv`

---

## 📁 1. Requirements

- Python 3.9+
- This project folder containing:
  - `cs463_final.ipynb`
  - `requirements.txt`
  - All datasets


---

## ⚙️ 2. Create a Virtual Environment

### **Windows**
```powershell
cd <path_to_cloned_repo>
python -m venv venv
venv\Scripts\activate
```

### **macOS / Linux**
```bash
cd ~<path_to_cloned_repo>
python3 -m venv venv
source venv/bin/activate
```

---

## 📦 3. Install Dependencies

With the venv activated:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

This installs:

- numpy, pandas, seaborn, matplotlib  
- scikit-learn, scipy  
- geopandas, shapely  
- xarray, requests  
- xgboost  
- plotly, wbdata, country_converter  
- ipykernel, ipython, nbformat, jupyter  

---

## 🧠 4. Register the Jupyter Kernel

This makes your virtual environment selectable inside Jupyter.

### **Windows**
```bash
python -m ipykernel install --user --name=climate-env --display-name "Climate Project Env"
```

### **macOS**
```bash
python3 -m ipykernel install --user --name=climate-env --display-name "Climate Project Env"
```

After this, you will see a kernel named:

```
Climate Project Env
```

---

## 📚 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

This opens a browser window.  
Open `cs463_final.ipynb`.

Then select your kernel:

```
Kernel → Change Kernel → Climate Project Env
```

---

## ▶️ 6. Run the Notebook

You may:

- Click **Run All**, or  
- Execute cells top to bottom manually.

All datasets must be in the **same folder** as the notebook.

