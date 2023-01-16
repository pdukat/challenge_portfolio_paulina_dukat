# Task 1
## Subtask 2
![](https://media.giphy.com/media/TEExkFeMOycBndLUPc/giphy.gif)
## Subtask 3
<p align="justify">
Hej! Wzięłam udział w chellange portfolio, bo szukam nowej ściezki kariery. Dzięki temu projektowi mam nadzieję przekonać się czy testowanie jest dla mnie (i czy jestem jeszcze w stanie się czegoś nauczyć :laughing:). A tak całkiem na poważnie, chciałabym zmienić branżę i liczę, że kurs da mi dobre podstawy do dalszego zgłębiania tajników testowania. W planach na ten rok mam znalezienie pracy w IT. 
</p>
Paulina

PS. z pewnych źródeł wiem, że są w grupie Robaczki Midasa :wink:

## Subtask 4
<p align="justify">
Aplikacja Scouts jest platformą skautingową służącą do zbierania i przedstawiania danych o zawodnikach piłkarskich. Pozwala na stworzenie indywidualnych profili graczy i przedstawienie ich występów w poszczególnych meczach. Umożliwia bardzo dokładne prześledzenie gry zawodnika w poszczególnym meczu i przedstawienie jego wyników w zbiorczym raporcie. 

<p align="justify">
Interfejs aplikacji jest prosty, i dość chaotyczny. Na pierwszy rzut oka użytkownika wybijają się statystyki, które po kliknięciu nie wywołują akcji – stanowią więc jedynie treść informacyjną. Zastanowić się można, czy skoro same w sobie nie stanowią żadnej funkcji to czy powinny zajmować czołowe miejsce na głównej stronie aplikacji. Nie można oprzeć się wrażeniu, że główny panel jest niejako pozbawiony treści – wszystko co aplikacja ma do zaoferowania jest ukryte w odnośnikach.
Z poziomu głównego panelu aplikacji użytkownik ma możliwość dodać profil nowego gracza, skontaktować się z zespołem twórcow i sprawdzić ostatnie aktywności w aplikacji. Z tego poziomu dostępne są również 4 zakładki, za pomocą których użytkownik może wylogować się z aplikacji, zmienić/wybrać język wyświetlania strony na angielski lub polski, wrócić do strony głównej i przejść do listy graczy dostępnych w systemie. Główny panel jest prosty i intuicyjny, sprawia jednak wrażenie, że aplikacja jest mocno ograniczona i nie oferuje nam zbyt dużo funkcjonalności. Najważniejsza jej funkcja, czyli podgląd wyników zawodnika jest bowiem "ukryta" i o mozliwości wygenerowania raportu uzytkownik dowiaduje się dopiero po wybraniu konkretnego zawodnika.  
Zakładka gracze oferuje najwięcej funkcji. Pojawia się pytanie, czy jej zawartość nie powinna być dostępna bezpośrednio z poziomu panelu głównego, tak aby wchodząc w aplikację użytkownik od początku nie miał wątpliwości do czego ona służy. Funkcja dodawania nowego zawodnika nie wydaje się najważniejszą w aplikacji, a własnie przegląd graczy i ich wyników. 
Z poziomu zakładki Gracze użytkownik ma możliwość przeglądu dostępnych zawodników, pobrania i wydrukowania ich listy, przefiltrowania tabeli pod kątem imienia, nazwiska, wieku, pozycji, klubu i oceny zawodnika, a także zmiany wyglądu tabeli wskazując interesujące go kolumny oraz wyszukanie konkretnego zawodnika. 
W panelu dodaj gracza formularz dodawania nowego zawodnika pozwala na podanie nieprawdziwych danych, tj. niemozliwych do spełnienia lub nic nie mówiących:
- znaków specjalnych w polu imienia i nazwiska,
- liter i znaków specjanych w liczbie pow. 12 (prefix+numer) w polu numeru telefonu,
- ujemnej wagi i ujemnego wzrostu, dane te mogą przekraczać trzyliczbową cyfrę, w tych polach można dodać również literę e, jednak przy próbie dodania zawodnika pojawia się odpowiedź ze strony aplikacji, aby wprowadzić liczbę
- datę urodzenia można wpisać ręcznie z klawiatury, przy czym pole roku może być nawet 6cyfrową liczbą
- pola poziom rozgrywek, główna pozycja i pozycja alternatywna powinny być moim zdaniem wybierane przez dropdown, liczba poziomów rozgrywek, podobnie jak liczba i rodzaje pozycji na boisku są ograniczone, pozostawienie wolnego pola pozwala na wpisywanie haseł nie mających odzwierciedlenia w rzeczywistości, np. znaków specjalnych 
- w polu języki można wpisać hasło nie będące określeniem na język, to pole również powinno być moim zdaniem wybierane przez dropdown
- hasło "łączy nas piłka" i "90 minut" są dla mnie niejasne, nie mam pewności o jaką informację chodzi
- dodając link youtube można wpisać hasło nie będące adresem url 
- Formularz nie wskazuje adresu e-mail jako pola koniecznego do wypełnienia, jednocześnie bez jego wypełnienia nie da się dodać nowego zawodnika 

<p align="justify"> Ponadto, pole adresu e-mail pozwala na dodanie hasła bez formatu adresu mailowego (bez @), jednocześnie bez jego prawidłowego formatu nie da się dodać nowego zawodnika, a formularz nie zwraca informacji użytkownikowi co jest nie tak w jego wypełnieniu.Devtoolsy zwracają nam informację o wystąpieniu błędu 500 - wewnętrznego błędu serwera. 
<p align="justify">
Wybór konkretnego gracza ujawnia w zakładkach kolejne funkcje aplikacji w postaci zakładek Mecze i Raporty. 
Zakładka mecze umożliwia dodanie nowego meczu rozegranego przez zawodnika, przegląd meczy dodanych dotychczasowo, a także ich edycję i dodanie raportu. 
 W panelu dodawania meczu występuje podoba sytuacja co w przypadku panelu dodawania gracza, czyli formularz pozwala na podanie nieprawdziwych danych: 
 
- ujemnej liczby zdobytych i straconych goli, w tych polach można dodać również literę e, jednak przy próbie dodania zawodnika pojawia się odpowiedź ze strony aplikacji, aby wprowadzić liczbę większą lub równą 0
- datę można wpisać ręcznie z klawiatury, przy czym pole roku może być nawet 6cyfrową liczbą. W przypadku wypełnienia wszystkich wymaganych pól w konfiguracji wlaśnie z takim 6cyfrowym rokiem przy próbie dodania meczu wyskakuje błąd, jednak formularz nie zwraca informacji użytkownikowi co jest nie tak w jego wypełnieniu. Devtoolsy zwracają nam informację o wystąpieniu błędu 500 - wewnętrznego błędu serwera. 
- kolor koszulki i liga powinny być moim zdaniem wybierane przez dropdown, pozostawienie wolnego pola pozwala na wpisywanie haseł nie mających odzwierciedlenia w rzeczywistości, np. znaków specjalnych
- pole czas gry pozwala na dodanie wartości większej niż 120 minut 
- pole wyboru meczu domowy/wyjazdowy nie jest oznaczone jako wymagane, a pozostawienie nie zaznaczonej żadnej z tych pozycji oznacza automatycznie mecz wyjazdowy po kliknięciu przycisku submit. 

<p align="justify"> Raport dotyczący występu i wyników zawodnika w poszczególnym meczu jest generowany na podstawie przebiegu meczu wprowadzonego za pomocą akcji „rozpocznij mecz”. Tam, w czasie rzeczywistym trwania meczu użytkownik wprowadza dane związane z występem zawodnika podczas przebiegu gry, ze wskazaniem miejsca na boisku, w którym zdarzenie wystąpiło. Funkcja ta jest jednak nieintuicyjna, dostępne w górnej części panelu przyciski nie są opisane, w związku z czym użytkownik musi kliknąć każdy z nich, celem sprawdzenia co wywołuje. Brakuje też możliwości przejścia do konkretnej minuty meczu lub przyspieszenia czasu. W obecnej formie użytkownik wprowadzając dane np. bramkarza, który w czasie trwania meczu nie ma tak częstego kontaktu z piłką jak pozostali zawodnicy, musi czekać bezczynnie aż upłynie czas do konkretnego zdarzenia z udziałem zawodnika, co wydaje się być na dłuższą metę frustrujące. Inną kwestią jest brak możliwości wyboru wszystkich możliwych zdarzeń, np. przewidzianych typowo dla bramkarza, jak obrona strzału na bramkę lub jej brak.
Mecz, który po wprowadzeniu danych nie zostanie zapisany przez użytkownika, pojawia się na stronie głównej z odnośnikiem powrotu do raportu, jednak przycisk ten nie wywołuje żadnej akcji. 
W zakładce raporty użytkownik ma możliwość przejrzeć i edytować raporty wygenerowane na podstawie poszczególnych meczów. Część danych potrzebnych do raportu jest automatycznie przetwarzana na podstawie wprowadzonych informacji z meczu, a część wymaga edycji, w postaci tekstowej, subiektywnej oceny zawodnika, do której służą proste edytory tekstu, dzięki którym można zmienić rodzaj i rozmiar czcionki, pogrubić tekst, podkreślić go, napisać kursywą, zacytować oraz wypunktować, a także cofnąć i powtórzyć ostatnie działanie. Edytor jest prosty i intuicyjny. 

<p align="justify">
Aplikacja jest dostosowana do urządzeń mobilnych. Nie umożliwia jednak porównywania do siebie zawodników, co z pewnością ułatwiłoby np. podjęcie decyzji o wyborze zawodnika na daną pozycję. Do ogólnej oceny zawodnika przydałaby się funkcja robienia raportu zbiorczego, na podstawie wszystkich rozegranych meczów.
<p align="justify">
Aplikacja jest w teorii dostępna w dwóch wersjach językowych - polskiej i angielskiej, jednak w polskiej wersji nie wszystkie pola są przetłumaczone, np. przeciski "submit" i "clear", pola "Web match" i "General" w formularzu dodawania meczu, przyciski "download CSV", "print", "view columns", "filter table" w zakładce gracze, czy opisy przycisów w edytowanym raporcie.   




