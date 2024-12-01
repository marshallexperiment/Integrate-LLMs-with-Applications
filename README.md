# Integrasi LLM dengan Aplikasi
<p align="center">
  <img src="https://img.shields.io/badge/python-%20-blue.svg?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Anaconda-%20-blue.svg?logo=anaconda&logoColor=white" alt="Anaconda">
</p>

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
Pertanyaan/Pesan: Tulislah sebuah paragraf tentang ibu kota Prancis.
Jawaban: Terletak di sebelah timur Prancis, Paris adalah ibu kota Prancis. Ini juga merupakan kota dengan populasi terbanyak di Prancis dengan jumlah penduduk 2,2 juta orang. Ini adalah pusat parlemen Prancis, Majelis Nasional. Kota ini terletak di jantung Prancis dan dikelilingi oleh wilayah Île-de-France.
---------------------------------------------------------------------------
C:\Users\ACAL\anaconda3\Lib\site-packages\ibm_watson_machine_learning\foundation_models\utils\utils.py:273: LifecycleWarning: Model 'meta-llama/llama-2-13b-chat' dalam status kadaluarsa dari 26 Agustus 2024 sampai tidak ditentukan. ID model alternatif: Tidak ada. Rincian lebih lanjut: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-lifecycle.html?context=wx&audience=wdp
warnings.warn(default_warning_template.format(
---------------------------------------------------------------------------
Prompt:
 Dari keluhan pelanggan berikut, ekstrak 3 faktor yang menyebabkan pelanggan tidak puas.
 Tulis masing-masing faktor pada baris baru.

 Keluhan pelanggan:
         Saya baru saja mencoba memesan penerbangan di situs web Anda yang sangat lambat. Semua
         waktu dan harga membingungkan. Saya suka bisa membandingkan
         fasilitas di kelas ekonomi dengan kelas bisnis berdampingan. Tetapi saya
         tidak pernah bisa memesan tempat duduk karena saya tidak mengerti peta tempat duduk.
         Lain kali, saya akan menggunakan agen perjalanan!

Daftar bernomor dari semua faktor yang menyebabkan pelanggan tidak puas:

Daftar keluhan:
 1. Situs web lambat
 2. Waktu dan harga membingungkan
 3. Ketidakpahaman terhadap peta tempat duduk
---------------------------------------------------------------------------
--------------------------Pemanggilan dengan REST-------------------------------------------
Pertanyaan/Pesan: Tulislah sebuah paragraf tentang ibu kota Prancis.
Jawaban: Paris adalah ibu kota Prancis dan pusat pemerintahan Republik Prancis. Kota ini terletak di jantung wilayah Ile-de-France, dan penduduknya disebut Parisien. Nama resmi kota ini adalah "Paris" (dalam bahasa Prancis) atau "Roubaix" (dalam bahasa Occitan).
---------------------------------------------------------------------------
