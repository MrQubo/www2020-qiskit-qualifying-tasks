# Instalacja – virtualenv (zalecane na Linuksie)

## Wymagania

- python3
- python3-virtualenv
- przeglądarka internetowa (Firefox, Chrome, Safari)

### Instalacja pythona i virtualenva

Pythona i virtualenva należy zainstalować z systemowego package managera. Np.:
```sh
sudo apt install python3 python3-virtualenv
```

Jeżeli virtualenva **nie ma** w systemowym package managerze, można go też zainstalować z pip-a (należy wtedy samemu pamiętać o aktualizacji virtualenva):
```sh
sudo pip3 install --upgrade pip
sudo pip3 install --upgrade virtualenv
```


## Tworzenie i aktywowanie virtualenva

W katalogu z repozytorium uruchamiamy:

### Linux (bash lub zsh)

```sh
python3 -m venv venv --prompt qiskit
source venv/bin/activate
```
Zamiast `qiskit` można wpisać dowolną wybraną nazwę.

### Inne powłoki i platformy

[https://docs.python.org/3/library/venv.html#creating-virtual-environments](https://docs.python.org/3/library/venv.html#creating-virtual-environments)


## Instalacja zależności

```sh
pip install --upgrade pip
pip install --upgrade -r requirements.txt
```


## Uruchomienie jupytera

```sh
jupyter lab
```

Automagicznie powinna otworzyć się przeglądarka internetowa.
Jeśli nie, to trzeba otworzyć, w przeglądarce, jeden z linków wyświetlonych w konsoli przez jupytera.

W jupyter'rze należy zacząć od otworzenia notatnika `index.ipynb` z przeglądarki plików po lewej stronie.
Znajdują się tam dalsze instrukcje.



# Instalacja – anaconda (zalecane na Windowsie)

## Wymagania

- anaconda
- przeglądarka internetowa (Firefox, Chrome, Safari)

### Instalacja anacondy

Pobieramy i instalujemy anacondę (Python 3.7) zgodnie z instrukcjami: [https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/).


## Tworzenie i aktywowanie środowiska condy

Na Windowsie otwieramy program „Anaconda Prompt”, na innych systemach – terminal. Następnie wykonujemy poniższe komendy:

```sh
conda update conda
conda create --name qiskit python=3
conda activate qiskit
```
Zamiast `qiskit` można wpisać dowolną wybraną nazwę.


## Instalacja zależności

W katalogu z repozytorium uruchamiamy:

```sh
conda install -c conda-forge --file requirements-conda-forge.txt
pip install --upgrade -r requirements-conda-pip.txt
```


## Uruchomienie jupytera

```sh
jupyter lab
```

Automagicznie powinna otworzyć się przeglądarka internetowa.
Jeśli nie, to trzeba otworzyć, w przeglądarce, jeden z linków wyświetlonych w konsoli przez jupytera.

W jupyter'rze należy zacząć od otworzenia notatnika `index.ipynb` z przeglądarki plików po lewej stronie.
Znajdują się tam dalsze instrukcje.



# Kontakt

Jeśli są jakieś problemy z instalacją, jupyterem lub dostarczonymi notatnikami można (a nawet trzeba) się ze mną skontaktować przez dowolny z poniższych kanałów:

#### Telegram
[@mrqubo](https://t.me/mrqubo)

#### Discord
MrQubo#2852

#### Email
[j.nowak26+www2020@student.uw.edu.pl](mailto:j.nowak26+www2020@student.uw.edu.pl)
