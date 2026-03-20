# dexp1
Docker experiments 1 repository


Obraz zawiera najnowsze ubuntu i je aktualizuje

Instalowany jest w nim też i uruchamiany apache.
Mozliwe jest rowniez zobaczenie prostej testowej strony internetowej

Aby zmniejszyć liczbę warstw w konenerze komendy są zgrupowane w jednym RUN.

#///////////////////////Komendy///////////////////////////////////

#Aby zbudować kontener - potrzebne są pliki Dockerfile1 i index.html
#(komenda wykoanana w foderze gdzie znajdują się oba pliki)
docker build -f Dockerfile1 -t web100 .

#wersja na repozytorium
docker build -f Dockerfile1 -t jk11111/dexp1:v1.0.0 .


#Aby uruchomić konetener:
docker run -d -p 8080:80 web100
