# Analiza zbioru Liver Disorders (BUPA) 🧬

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-brightgreen)](https://pandas.pydata.org/)

## 📋 Opis projektu
Projekt realizowany w ramach przedmiotu **Analiza Danych**. Celem analizy jest klasyfikacja grup diagnostycznych pacjentów (zmienna `selector`) na podstawie wyników badań krwi oraz spożycia alkoholu. Zbiór danych pochodzi z repozytorium **UCI Machine Learning** i dotyczy zaburzeń wątroby u mężczyzn.

---

## 🏗️ Struktura Projektu (Zgodnie z wymaganiami)

### 1. Opis problemu
* **Zbiór danych:** BUPA Liver Disorders.
* **Cechy:** 5 testów krwi (mcv, alkphos, sgpt, sgot, gammagt) + liczba "drinków" na dobę.
* **Źródło:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/60/liver+disorders).

### 2. Opis danych
* Analiza statystyk opisowych (średnie, odchylenia standardowe).
* Wizualizacja korelacji oraz rozkładów zmiennych (użycie bibliotek `matplotlib` i `seaborn`).

### 3. Przygotowanie danych
* **Czyszczenie:** Usunięcie duplikatów (zidentyfikowano kluczowe powtórzenia wierszy, np. 84 i 86).
* **Transformacje:** Skalowanie cech oraz obsługa specyfiki małego zbioru danych (ok. 345 instancji).

### 4. Tworzenie modelu i ocena
W projekcie wykorzystano algorytmy uczenia maszynowego w środowisku Python:
* **Random Forest Classifier** (Model bazowy)
* **Grid Search CV** (Optymalizacja hiperparametrów)
* **Porównanie wyników:** Poprawa dokładności z **71% na 75%** po dostrojeniu parametrów.

### 5. Podsumowanie
* Zbiór BUPA jest wyzwaniem ze względu na nieliniowość i małą liczbę próbek.
* Kluczowym elementem poprawy wyniku była eliminacja duplikatów i precyzyjny tuning lasu losowego.

---

## 🛠️ Technologie
* **Jupyter Notebook**
* **Python** (Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib)

### Zainstaluj wymagane biblioteki
pip install pandas matplotlib seaborn scikit-learn