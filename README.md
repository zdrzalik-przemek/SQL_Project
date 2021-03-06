# SQL-Hospital

Baza danych dla szpitala
Diagram:

![diagram](https://github.com/ZdrzalikPrzemyslaw/SQL-Hospital/blob/master/.github/Database_diagram.png)

Zalozenia:

1. Pacjenci są rejestrowani na określony okres, w określonym oddziale. 
2. W szpitalu pracują lekarze różnych specjalności
3. Pacjent jest pod opieką (ma przypisanego) lekarza rodzinnego.
Też lekarzami rodzinnymi
4. Pacjent może zapisać się na wizytę do dowolnego lekarza na określony dzień i godzinę
5. W ramach każdej specjalności lekarz pacjent ma założoną kartę, na której zapisuje się przebieg leczenia: daty wizyt i zalecenia.
6. Lekarze są pracownikami oddziałów. Jeden z lekarzy jest ordynatorem danego oddziału. Lekarze posiadają szefów, którzy również są lekarzami.
7. Każdy Lekarz przyjmuje pacjenta w swoim gabinecie.
8. Gabinety mogę znajdować się w różnych oddziałach (nr gabinetu jest unikalny dla oddziału).
9. W każdym budynku znajduje się co najmniej jeden oddział
10. Każdy oddział posiada swoje wyposażenie w konkretnej liczbie
11. W skład wyposażenia wchodzi przedmiot posiadający swój unikalny numer oraz nazwę
12. Każdy przedmiot jest dostarczany okresowo przez konkretnego dostawcę po określonej cenie
13. Każdy dostawca pochodzi z konkretnego kraju oraz jest z nim podpisana aktualna umowa 
14. Każda umowa ma swoją datę oraz unikalny numer i przypisane są do niej przedmioty, których ona dotyczy
15. Rekordy wszystkich umów zapisane są w historii transakcji


Zapytania:

1.	Wyświetl nazwiska, identyfikatory specjalizacji i datę urodzenia dla lekarzy o nazwisku Nazwisko1 oraz Nazwisko2. Wynik posortuj rosnąco. 
2.	Dla każdego ordynatora wyświetl jego nazwisko, datę rozpoczęcia kadencji oraz datę podwyżki. Data podwyżki (z etykietą kiedy) to pierwszy poniedziałek po sześciu miesiącach trwania kadencji.
3.	Wyświetl nazwiska, identyfikator specjalizacji, numer oddziału dla pracowników pracujących w najstarszym budynku.
4.	Wyświetl dla każdego lekarza jego nazwisko, numer oddziału oraz nazwiska wszystkich lekarzy, którzy pracują razem z nim w tym samym oddziale. Nazwij odpowiednio każdą z kolumn.
5.	Wyświetl imiona i nazwiska pracowników, których ordynator oddziału ma na nazwisko Nazwisko.
6.	Wyświetl nazwiska, wynagrodzenie oraz numer telefonu dla tych lekarzy, którzy mają numer telefonu.
7.	Wyświetl imiona i nazwiska tych lekarzy, których trzecią literą nazwiska jest ‘a’. Rezultat nazwij lekarze i przedstaw w postaci jednego ciągu, np. Jan Kowalski
8.	Wyświetl imiona z nazwiskami, numery oddziałów oraz identyfikatory stanowisk dla pracowników z budynku 1.
9.	Podaj numer oddziału i najniższą płacę w oddziale, dla oddziału z najwyższym średnim wynagrodzeniem.
10.	Podaj imiona i nazwiska oraz daty rozpoczęcia kadencji ordynatorów, którzy rozpoczęli kadencję w roku, w którym wybudowano najwięcej budynków.
11.	Wyświetl nazwiska oraz imiona trzech najlepiej zarabiających lekarzy.
12.	Podaj imiona, nazwiska i roczną płacę lekarzy wraz z odpowiednim aliasem.
13.	Podaj imiona, nazwiska, specjalności i płace lekarzy, którzy zarabiają poniżej średniej w swoim oddziale.
14.	Podaj ilu lekarzy pracuje w każdym oddziale o specjalności Mikrobiologia lekarska.
15.	Podaj naziwska i id ordynatorów oraz ile wynosi różnica między ich zarobkami a średnią płacą w całym szpitalu.
16.	Wyświetl nazwiska lekarzy, którzy miesięcznie zarabiają pomiędzy 3000 a 9000 PLN.
17.	Podaj ID budynku, w którym nie zatrudnia się lekarzy o specjalnosci Mikrobiologia lekarska.
18.	Podaj nazwiska pacjentów, których lekarzem rodzinnym jest Jan Kowalski
19.	Wyświetl nazwiska pacjentów, którzy przebywali w szpitalu w pierwszym tygodniu maja dłużej niż 1 dzień.
20.	Wyświetl wszystkie kobiety, które przebywają aktualnie w szpitalu wraz z ich zaleceniami oraz przypisanym lekarzem rodzinnym.
21.	Wyświetl lekarza, któremu należy się podwyżka, czyli takiego który wykonał najwięcej wizyt oraz zarabia mniej niż średnia w jego oddziale.
22.	Wyświetl lekarzy, którzy pracują w budynku, w którym stawka godzinowa jest średnio najniższa.
23.	Wyświetl nazwę oddziału, w którym Lampy Dezynfekcyjne do Sterylizacji Pomieszczeń stanowią mniej niż 10% całego wyposażenia.
24.	Wyszukaj wszystkich lekarzy wraz z przypisanym im gabinetem, oddziałem, budynkiem, którzy są mikrobiologami
25.	Wyszukaj wszystkich lekarzy, którzy mieli styczność z zarażonym pacjentem X.
26.	Wyświetl umowy, które trwały więcej niż miesiąc i zakończyły się.
27. 	Znajdź Oddział na którego zaopatrzenie wydaje się najwiecej pieniędzy.
28. 	Znajdź budynek który ma najwięcej zaopatrzenia (suma ilości wszyskich przedmiotów)
29. 	Wyświetl najpopularniejszy dzien przyjec do szpitala
30. 	Wyświetl hierarchię Szpitala (od głownych szefów, po ich 'podwładnych')
31. 	Wyświetl wszystkich lekarzy zarabiających mniej, niż minimalna stawka dla ich specjalności.
32. 	Znajdź dostawców, którzy dostarczają do wszystkich oddziałów.

