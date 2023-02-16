# Projects

Projekt 1 - SQL
1. Stwórz Bazę „Sklep odzieżowy”

2. Utwórz tabelę „Producenci” z kolumnami:

id producenta
nazwa producenta
adres producenta
nip producenta
data podpisania umowy z producentem
Do każdej kolumny ustaw odpowiedni „constraint”

3. Utwórz tabelę „Produkty” z kolumnami:

id produktu
id producenta
nazwa produktu
opis produktu
cena netto zakupu
cena brutto zakupu
cena netto sprzedaży
cena brutto sprzedaży
procent VAT sprzedaży
Do każdej kolumny ustaw odpowiedni „constraint”

4. Utwórz tabelę „Zamówienia” z kolumnami:

id zamówienia
id klienta
id produktu
Data zamówienia
Do każdej kolumny ustaw odpowiedni „constraint”

5. Utwórz tabelę „Klienci” z kolumnami:

id klienta
id zamówienia
imię
nazwisko
adres
Do każdej kolumny ustaw odpowiedni „constraint”
 
6. Połącz tabele ze sobą za pomocą kluczy obcych:

Produkty – Producenci
Zamówienia – Produkty
Zamówienia - Klienci

7. Każdą tabelę uzupełnij danymi wg:

Tabela „Producenci” – 4 pozycje
Tabela „Produkty” – 20 pozycji
Tabela „Zamówienia” – 10 pozycji
Tabela „Klienci” – 10 pozycji
8. Wyświetl wszystkie produkty z wszystkimi danymi od producenta który znajduje się na pozycji 1 w tabeli „Producenci”

9. Posortuj te produkty alfabetycznie po nazwie

10. Wylicz średnią cenę za produktu od producenta z pozycji 1

11. Wyświetl dwie grupy produktów tego producenta:

Połowa najtańszych to grupa: „Tanie”
Pozostałe to grupa: „Drogie”
12. Wyświetl produkty zamówione, wyświetlając tylko ich nazwę

13. Wyświetl wszystkie produkty zamówione – ograniczając wyświetlanie do 5 pozycji

14. Policz łączną wartość wszystkich zamówień

15. Wyświetl wszystkie zamówienia wraz z nazwą produktu sortując je wg daty od najstarszego do najnowszego

16. Sprawdź czy w tabeli produkty masz uzupełnione wszystkie dane – wyświetl pozycje dla których brakuje danych

17. Wyświetl produkt najczęściej sprzedawany wraz z jego ceną

18. Znajdź dzień w którym najwięcej zostało złożonych zamówień



Projekt 2 - ML
Projekt końcowy

Lending Club to firma pożyczkowa typu peer-to-peer, która łączy pożyczkobiorców z inwestorami za pośrednictwem platformy internetowej. Obsługuje osoby, które potrzebują pożyczek osobistych w wysokości od 1000 do 40 000 USD. Pożyczkobiorcy otrzymują pełną kwotę udzielonej pożyczki pomniejszoną o opłatę początkową, która jest uiszczana firmie. Inwestorzy kupują weksle zabezpieczone osobistymi pożyczkami i płacą Lending Club opłatę za usługę. Firma Lending Club udostępnia dane o wszystkich pożyczkach udzielonych za pośrednictwem swojej platformy w określonych okresach. 
Na potrzeby tego projektu zostały użyte dane dotyczące pożyczek udzielonych za pośrednictwem Lending Club na przestrzeni lat 2007 -2011. Każda pożyczka jest opatrzona informacją o tym, czy ostatecznie została spłacona (Fully Paid lub Charged off w kolumnie loan_status). Twoim zadaniem jest zbudowanie modelu klasyfikacyjnego, który na podstawie tych danych będzie przewidywał z określoną dokładnością, czy potencjalny pożyczkobiorca spłaci swój dług z tytułu zaciągniętej pozyczki. Do zbioru danych dołączony jest plik z opisem wszystkich zmiennych oraz plik „FICO Score ranged.pdf”, w którym dokładnie opisano znaczenie jednej z kolumn.

Poniżej zaprezentowane są poszczególne etapy analizy, których wykonanie jest konieczne do zaliczenia projektu oraz ich punktacja:
1.	Obróbka danych (Data Processing) (70pkt) – jako doświadczony Data Scientist zapewne znasz poszczególne kroki, które należy wykonać na tym etapie, więc nie będziemy ich tutaj wyszczególniać.
2.	EDA, czyli obszerna eksploracja danych (100pkt) Opisz wnioski płynące z każdego wykresu, swoje hipotezy poprzyj testami statystycznymi takimi jak np. t-test lub Chi-square. Dodatkowo odpowiedz na poniższe pytania:
1.	W jaki sposób wynik FICO wiąże się z prawdopodobieństwem spłacenia pożyczki przez pożyczkobiorcę?
2.	W jaki sposób wiek kredytowy wiąże się z prawdopodobieństwem niewykonania zobowiązania i czy ryzyko to jest niezależne lub związane z wynikiem FICO
3.	W jaki sposób status kredytu hipotecznego na dom wiąże się z prawdopodobieństwem niewypłacalności?
4.	W jaki sposób roczny dochód wiąże się z prawdopodobieństwem niewykonania zobowiązania?
5.	W jaki sposób historia zatrudnienia wiąże się z prawdopodobieństwem niewykonania zobowiązania?
6.	Jak wielkość żądanej pożyczki jest powiązana z prawdopodobieństwem niewykonania zobowiązania?
3.	Feature Engineering – utwórz 20 nowych zmiennych (60 pkt)

4.	Modelowanie (150 pkt)
1.	Wykonaj klasteryzację danych (wypróbuj do tego celu kilka metod, min. 3) i sprawdź, czy występują jakieś segmenty pożyczkobiorców, wykorzystaj odpowiednie metody do określenia optymalnej liczby klastrów (40 pkt)
2.	Wytrenuj 5 różnych modeli, wykorzystując do każdego inny algorytm, a następnie porównaj ich działanie, za metrykę oceny jakości modelu przyjmij AUROC score. (50pkt)
3.	Sprawdź działanie wcześniej użytych metod na skompresowanych danych za pomocą PCA, porównaj wyniki (AUROC score) z modelami wytrenowanymi w poprzednim podpunkcie. (20pkt)
4.	Zbuduj finalny model, którego AUROC score będzie >= 80%, pamiętaj o doborze istotnych zmiennych, kroswalidacji oraz dostrojeniu parametrów modelu, pomyśl również o zbalansowaniu klas. (40pkt)

Za całość do zdobycia jest 380 punktów. Do zaliczenia projektu potrzeba minimum 300 pkt.
