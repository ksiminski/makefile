# [EN] simple makefile generator for C/C++ [PL] prosty generator plików makefile dla C/C++ 

## English version 

### operating system

It works for unix/linux OS.

### prerequisites

The script uses: ```bash```, ```awk```.

### usage

Run in your C/C++ sources folder:

```$ ./generator-makefile.sh```

The script searches recursively for the files ```*.cpp``` and ```*.c```. It creates a ```makefile``` file. If the file already exists, the previous version will be saved to the ```makefile-old``` file.

### makefiles

Options in the ```makefile``` file:

* ```make``` or ```make release```
   compiles in release mode and runs the compiled file. Creates a ```_release``` folder and saves the binary files there.

* ```make debug```
   compiles in debug mode and runs in the valgrind environment. Creates a ```_debug``` folder and saves the binary files there.

* ```make gprof```
   compiles in debug mode, runs the gprof profiler and writes its result to the standard output.

* ```make clean``` removes binary files (```*.o``` and ```main```) along with the ```_release``` and ```_debug``` folders.

* ```make 5-minutes``` removes binary files (```*.o``` and ```main```) from the ```_release``` and ```_debug``` folders not older than 5 minutes.

* ```make 10-minutes``` removes binary files (```*.o``` and ```main```) from the ```_release``` and ```_debug``` folders not older than 10 minutes.

* ```make 30-minutes``` removes binary files (```*.o``` and ```main```) from the ```_release``` and ```_debug``` folders not older than 30 minutes.

* ```make 60-minutes``` removes binary files (```*.o``` and ```main```) from the ```_release``` and ```_debug``` folders not older than 60 minutes.

* ```make 1-days``` removes binary files (```*.o``` and ```main```) from the ```_release``` and ```_debug``` folders not older than 1 day.

* ```make doxygen``` starts the ```doxygen``` program.

## wersja polska

### system operacyjny

Skrypt działa w uniksie/linuksie.

### wymagania

Skrypt korzysta z ```bash```a i ```awk```.

### użycie

Uruchom w folderze ze źródłami w C/C++:

```$ ./generator-makefile.sh```

Skrypt wyszukuje rekurencyjnie pliki ```*.cpp``` i ```*.c```. Tworzy plik ```makefile```.  Jeżeli plik już istnieje, poprzednia wersja zostanie zapisana do pliku ```makefile-old```.

### makefile

Opcje w pliku ```makefile```:

* ```make``` lub ```make release``` 
  kompiluje w trybie release i uruchamia skompilowany plik. 
  Tworzy folder ```_release``` i tam zapisuje pliki binarne.

* ```make debug```
  kompiluje w trybie debug i uruchamia w środowisku ```valgrind```.
Tworzy folder ```_debug``` i tam zapisuje pliki binarne.

* ```make gprof```
  kompiluje w trybie debug, uruchamia profiler gprof i wypisuje jego wynik na standardowe wyjście.

* ```make clean``` usuwa pliki binarne (```*.o``` i ```main```) wraz z folderami ```_release``` i ```_debug```.

* ```make 5-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 5 minut.

* ```make 10-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 10 minut.

* ```make 30-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 30 minut.

* ```make 60-minutes``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 60 minut.

* ```make 1-days``` usuwa pliki binarne (```*.o``` i ```main```) z folderów ```_release``` i ```_debug``` nie starsze niż 1 dzień.

* ```make doxygen``` uruchamia program ```doxygen```.

