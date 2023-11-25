# simple makefile generator for g++ / c++

Bardzo prosty generator plików makefile dla C/C++. 

# użycie

Uruchom w folderze ze źródłami w C/C++:

```$ ./generator-makefile.sh```

Skrypt wyszukuje rekurencyjnie pliki ```*.cpp``` i ```*.c```.

Po uruchomieniu zostanie wygenerowany plik ```makefile```.
Jeżeli plik już istniał, poprzednia wersja zostanie zapisana do pliku ```makefile-old```.

# makefile

Opcje w pliku ```makefile```:

* ```make``` lub ```make release``` 
  kompiluje w trybie release i uruchamia skompilowany plik. 
  Tworzy folder ```_release``` i tam zapisuje pliki binarne.

* ```make debug```
  kompiluje w trybie debug i uruchamia w środowisko valgrind.
Tworzy folder ```_debug``` i tam zapisuje pliki binarne.

* ```make debug```
  kompiluje w trybie debug, uruchamia profiler gprof i wypisuje jego wynik na standardowe wyjście.

* ```make clean``` usuwa pliki binarne (```*.o``` i ```main```) wraz z folderami ```_release``` i ```_debug```.

* ```make 5-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 5 minut.

* ```make 10-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 10 minut.

* ```make 30-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 30 minut.

* ```make 60-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 60 minut.

* ```make 1-days``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 1 dzień.

* ```make doxygen``` uruchamia program ```doxygen```.




# 
