# ML_Project
Założeniem projektu było wykonanie modelu, który będzie rozpoznawał język danego tekstu (jeden z 20 języków). Projekt wykonany został na podstawie 3 jupyter notebooków z wykorzystaniem datasetu papluca/language-identification z HuggingFace. W pierwszym notebooku 1_dataset_load pobieram, analizuję dane, przygotowuję do dalszej obróbki oraz zapisuje dane. W drugim notebooku 2_embeddings dokonuję pobrania sentence transformera i transformuje dane a następnie zapisuje w pliku. W trzecim notebooku 3_classyfier tworzę model sieci neuronowej, dzielę dane z pliku na treningowe, walidacyjne i testowe, trenuję mój model i dokonuję jego walidacji (wyniki możliwe do obejrzenia w TensorBoardzie). Na samym końcu napisałem skrypt umożliwiający przetestowanie modelu oraz wyświetlenie wyników w porównaniu do prawidłowych danych.

Z danych dokładności predykcji modelu dla kolejnych epok wynika, że jego dokładność przy trenowaniu do 10 epok oscyluje od około 97,5 do 98,0 %.


#Instrukcje dotyczące niezbędnych kroków, które należy podjąć przed rozpoczęciem pracy na projekcie.


## Wymagania sprzętowe

Wirtualna maszyna z Ubuntu 22.04, preferowane 16G RAM


## W pierwszej kolejności prosze skolonować repozytorium
Kod źródłowy:
```shell 
git clone https://github.com/PPPASZKO/ML_Project_languages
cd ML_Project_languages
```

## Instalacja venv
Najpierw zainstaluj pakiety potrzebne do instalacji poprawnych wersji Pythona w systemie Ubuntu.
```bash
sudo apt-get update
sudo apt-get install curl python3-venv 
```

## Tworzenie środowiska Pythona
Sprawdź, czy wersja Pythona, której używamy, jest wyższa niż 3.7.

```shell 
python3 --version 
```

Jeśli tak, możemy przejść do tworzenia wirtualnego środowiska.

```shell 
python3 -m venv venv_ml_project
source venv_ml_project/bin/activate
```

Po aktywacji środowiska, twój prompt poinformuje cię o wirtualnym środowisku.

Instalujemy wymagane pakiety.
```shell
pip install -r requirements.txt 
```

Po zainstalowaniu Pakietów można uruchomić jupytera
```shell
jupyter notebook
```
