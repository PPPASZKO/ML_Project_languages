# ML_Project
Instrukcje dotyczące niezbędnych kroków, które należy podjąć przed rozpoczęciem pracy na projekcie.


## Wymagania sprzętowe

Wirtualna maszyna z Ubuntu 22.04, preferowane 16G RAM


## W pierwszej kolejności prosze skolonować repozytorium
Kod źródłowy:
```shell 
cd 
git clone https://github.com/PPPASZKO/ML_Project_languages
cd ML_Project
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
