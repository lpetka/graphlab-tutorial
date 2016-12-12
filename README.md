# GraphLab Tutorial

### Konfiguracja

1.  Pobieramy obraz dcokerowy

    ```
    docker pull rothnic/anaconda-notebook
    ```

1. Uruchamiamy kontener

    ```
    cd graphlab-tutorial
    docker run -v $(pwd)/nb:/home/condauser/notebooks/GraphLab -p 8888:8888 -i -t rothnic/anaconda-notebook
    ```

1. Jupyter Notebook jest dostępny pod adresem http://localhost:8888/

### GraphLab

1. Aby korzystać z graphlaba należy się zarejestrować na stronie https://turi.com/download/academic.html

2. Jeśli ktoś nie chce używać własnego maila to polecam użyć http://10minutemail.com/

### Instalowanie GraphLab po rejestracji 

1. Po otwarciu Jupyter Notebook klikamy na New -> Terminal i wykonujemy poniższe

2. Zmiana środowiska na python 2.7.x

    ```
    source activate python2
    ```

2. Zainstalowanie GraphLaba po rejestracji

    ```
    pip install --upgrade --no-cache-dir https://get.graphlab.com/GraphLab-Create/2.1/<email-address>/<product-key>/GraphLab-Create-License.tar.gz 
    ```