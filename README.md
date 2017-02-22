# Wstęp
ISA-RSM to projekt przygotowany na Olimpiadę Innowacji Technicznej. Celem projektu było przygotowanie makiety "nowoczesnego domu", która umożliwia sterowanie natężeniem oświetlenia, roletami, włączać/wyłączać urządzenia. Praca zajęła I miejsce w kategorii Usprawnienie Softwarowo-Techniczne na poziomie okręgowym w Poznaniu.

System składa się z trzech głównych podzespołów:
* część mikrokontrolerów i czujników
* część sterująca
* strona www umożliwiająca zdalne sterowanie

# Część mikrokontrolerów i czujników

System wykorzystuje mikrokontrolery AVR do sterowania układami automatyki (przekaźnikami, wyjściami analogowymi) oraz odczytu wartości czujników (moduł wejść optoizolowanych, wejścia analogowe, pomiar temperatury). Mikrokontrolery zostały zaprogramowanie przy pomocy języka BASCOM oraz wykorzystują port RS-485 do komunikacji z jednostką sterującą.

# Część sterująca

Jednostką sterującą jest oprogramowanie napisane w C++ na platformę komputerową Raspberry Pi z zainstalowanym systemem operacyjnym Raspbian Linux. Oprogramowanie wykorzystuję bazę danych MySQL do przechowywania wyników pomiarów oraz ustawień.
Warstwa interfejsu graficznego została napisana przy użyciu biblioteki Qt. Poniżej zamieszczam zrzuty ekranu z aplikacji: 

![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_1.png)
![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_2.png)
![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_3.png)
![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_4.png)
![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_5.png)

# Strona WWW

Całością systemu można sterować zdalnie przy pomocy witryny internetowej napisanej w PHP/JS/CSS:

![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_6.png)
![alt tag](https://github.com/mateuszradny/ISA-RSM/blob/master/screenshots/screenshot_7.png)


# Prezentacja

Krótki film ukazujący możliwości makiety:

[![Movie](https://img.youtube.com/vi/sFjCFTvsWlk/0.jpg)](https://www.youtube.com/watch?v=sFjCFTvsWlk)
