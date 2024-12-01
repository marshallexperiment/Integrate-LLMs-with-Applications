# Integrasi LLM dengan Aplikasi
<div align="center">
<img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
<img src="https://img.shields.io/badge/Anaconda-3670A0?style=for-the-badge&logo=anaconda&logoColor=white">
<img src="https://img.shields.io/badge/IBM%20Cloud-005C8E?style=for-the-badge&logo=ibmcloud&logoColor=white">
<img src="https://img.shields.io/badge/Streamlit-FF4B5C?style=for-the-badge&logo=streamlit&logoColor=white">
<img src="https://img.shields.io/badge/License-MIT-yellowgreen?style=for-the-badge&logo=opensource&logoColor=white">

</div>

Proyek ini menunjukkan cara mengintegrasikan Model Bahasa Besar (LLMs) ke dalam aplikasi menggunakan API Watson Machine Learning dari IBM Cloud. Proyek ini menggunakan Python dan Streamlit untuk membuat aplikasi sederhana yang berkomunikasi dengan IBM Watson ML API untuk melakukan berbagai tugas bahasa seperti pembuatan teks, penjawaban pertanyaan, dan ekstraksi data.

## Persyaratan

Sebelum memulai, pastikan Anda telah menginstal hal-hal berikut:

- **Lingkungan Anaconda**
- **Python**

### Library yang Diperlukan (dari `requirements.txt`):

```text
load_dotenv==0.1.0
ibm_watson_machine_learning==1.0.345
ibm-cloud-sdk-core==3.16.7
streamlit==1.31.0
python-dotenv==1.0.0
```

## Instalasi
Instal Anaconda dan konfigurasikan sebagai interpreter Python di VSCode atau IDE lainnya.
Buka IDE Anda dan gunakan Ctrl + Shift + P untuk memilih lingkungan Anaconda sebagai interpreter.

1. Clone Repository:

```bash
git clone https://github.com/username/Integrate_LLMs_with_applications.git
```
2. Pindah ke Direktori Proyek:

```bash
cd Integrate_LLMs_with_applications
```

3. Instal Dependensi: Jalankan perintah berikut untuk menginstal library yang diperlukan:

```bash
pip install -r requirements.txt
pip install ibm-watson-machine-learning
pip install ibm-cloud-sdk-core
pip install streamlit
```
4. Menjalankan Aplikasi
Untuk menjalankan skrip Python dan menggunakan API Watson Machine Learning, eksekusi:

```bash
python ./demo_wml_api.py
streamlit run demo_wml_api_with_streamlit.py
```

## Hasil
```bash
python demo_wml_api.py
---------------------------------------------------------------------------
Question/request: Write a paragraph about the capital of France.
Answer: Located in the east of France, Paris is the capital of France. It is also the most populated city of France with a population of 2.2 million people. It is the seat of the French parliament, the National Assembly. The city is located in the heart of France and is surrounded by the Île-de-France region.
---------------------------------------------------------------------------
C:\Users\LENOVO\anaconda3\Lib\site-packages\ibm_watson_machine_learning\foundation_models\utils\utils.py:273: LifecycleWarning: Model 'meta-llama/llama-2-13b-chat' is in deprecated state from 2024-08-26 until None. IDs of alternative models: None. Further details: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-lifecycle.html?context=wx&audience=wdp
warnings.warn(default_warning_template.format(
---------------------------------------------------------------------------
Prompt: 
 From the following customer complaint, extract 3 factors that caused the customer to be unhappy.
 Put each factor on a new line.

 Customer complaint:
         I just tried to book a flight on your incredibly slow website.  All
         the times and prices were confusing.  I liked being able to compare
         the amenities in economy with business class side by side.  But I
         never got to reserve a seat because I didn't understand the seat map.
         Next time, I'll use a travel agent!


 Numbered list of all the factors that caused the customer to be unhappy:


List of complaints: 1. Slow website
 2. Confusing times and prices
 3. Lack of understanding of the seat map
---------------------------------------------------------------------------
--------------------------Invocation with REST-------------------------------------------
Question/request: Write a paragraph about the capital of France.
Answer: Paris is the capital of France and the seat of government of the French Republic. The city is located in the heart of the Ile-de-France region, and its inhabitants are called Parisiens. The official name of the city is "Paris" (in French) or "Roubaix" (in Occitan).
---------------------------------------------------------------------------
```
