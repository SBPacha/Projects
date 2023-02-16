# Projects
Projects to CV

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
