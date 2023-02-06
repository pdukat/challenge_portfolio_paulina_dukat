# TASK 1
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
Interfejs aplikacji chociaż nie składa się z wielu elementów to jest dość chaotyczny. Na pierwszy rzut oka użytkownika wybijają się statystyki, które po kliknięciu nie wywołują akcji – stanowią więc jedynie treść informacyjną. Zastanowić się można, czy skoro same w sobie nie stanowią żadnej funkcji to czy powinny zajmować czołowe miejsce na głównej stronie aplikacji. Nie można oprzeć się wrażeniu, że główny panel jest niejako pozbawiony treści – wszystko co aplikacja ma do zaoferowania jest ukryte w odnośnikach.
Z poziomu głównego panelu aplikacji użytkownik ma możliwość dodać profil nowego gracza, skontaktować się z zespołem twórcow i sprawdzić ostatnie aktywności w aplikacji. Z tego poziomu dostępne są również 4 zakładki, za pomocą których użytkownik może wylogować się z aplikacji, zmienić/wybrać język wyświetlania strony na angielski lub polski, wrócić do strony głównej i przejść do listy graczy dostępnych w systemie. Główny panel jest prosty i intuicyjny, sprawia jednak wrażenie, że aplikacja jest mocno ograniczona i nie oferuje nam zbyt dużo funkcjonalności. Najważniejsza jej funkcja, czyli podgląd wyników zawodnika jest bowiem "ukryta" i o mozliwości wygenerowania raportu uzytkownik dowiaduje się dopiero po wybraniu konkretnego zawodnika.  
Zakładka gracze oferuje najwięcej funkcji. Pojawia się pytanie, czy jej zawartość nie powinna być dostępna bezpośrednio z poziomu panelu głównego, tak aby wchodząc w aplikację użytkownik od początku nie miał wątpliwości do czego ona służy. Funkcja dodawania nowego zawodnika nie wydaje się najważniejszą w aplikacji, a własnie przegląd graczy i ich wyników. 
Z poziomu zakładki Gracze użytkownik ma możliwość przeglądu dostępnych zawodników, pobrania i wydrukowania ich listy, przefiltrowania tabeli pod kątem imienia, nazwiska, wieku, pozycji, klubu i oceny zawodnika, a także zmiany wyglądu tabeli wskazując interesujące go kolumny oraz wyszukanie konkretnego zawodnika. Pobranie listy zawodników jest możliwe w formacie .csv, jednak część z danych w  tabeli nie wyświetla się prawidłowo. 
 
![KLIK TABELA](https://github.com/pdukat/chellange_portfolio_paulina_dukat/blob/main/321517830_698503938385027_501916212938117038_n.png)
 
 W panelu dodaj gracza formularz dodawania nowego zawodnika pozwala na podanie nieprawdziwych danych, tj. niemozliwych do spełnienia lub nic nie mówiących:</p> 

- znaków specjalnych w polu imienia i nazwiska,
- liter i znaków specjanych w liczbie pow. 12 (prefix+numer) w polu numeru telefonu,
- ujemnej wagi i ujemnego wzrostu, dane te mogą przekraczać trzyliczbową cyfrę, w tych polach można dodać również literę e, jednak przy próbie dodania zawodnika pojawia się odpowiedź ze strony aplikacji, aby wprowadzić liczbę
- datę urodzenia można wpisać ręcznie z klawiatury, przy czym pole roku może być nawet 6cyfrową liczbą
- pola poziom rozgrywek, główna pozycja i pozycja alternatywna powinny być moim zdaniem wybierane przez dropdown, liczba poziomów rozgrywek, podobnie jak liczba i rodzaje pozycji na boisku są ograniczone, pozostawienie wolnego pola pozwala na wpisywanie haseł nie mających odzwierciedlenia w rzeczywistości, np. znaków specjalnych 
- w polu języki można wpisać hasło nie będące określeniem na język, to pole również powinno być moim zdaniem wybierane przez dropdown
- hasło "łączy nas piłka" i "90 minut" nie wskazują wprost o jaką informację formularz prosi 
- dodając link youtube można wpisać hasło nie będące adresem url 
- Formularz nie wskazuje adresu e-mail jako pola koniecznego do wypełnienia, jednocześnie bez jego wypełnienia nie da się dodać nowego zawodnika 

<p align="justify"> Ponadto, pole adresu e-mail pozwala na dodwanie hasła w złym formacie. Po wpisaniu adresu e-mail w złym formacie (bez @) serwis nie pozwala na dodanie gracza, a formularz nie zwraca żadnej informacji wskazującej błędne miejsce.Devtoolsy zwracają nam informację o wystąpieniu błędu 500 - wewnętrznego błędu serwera. 
 
 ![alt text](https://github.com/pdukat/challenge_portfolio_paulina_dukat/blob/main/validemail.JPG?raw=true)
 
 ![alt text](https://github.com/pdukat/challenge_portfolio_paulina_dukat/blob/main/internalservererror.jpg.JPG?raw=true)
 
<p align="justify">
Wybór konkretnego gracza ujawnia w zakładkach kolejne funkcje aplikacji w postaci zakładek Mecze i Raporty. 
Zakładka mecze umożliwia dodanie nowego meczu rozegranego przez zawodnika, przegląd meczy dodanych dotychczasowo, a także ich edycję i dodanie raportu. 
 W panelu dodawania meczu występuje podoba sytuacja co w przypadku panelu dodawania gracza, czyli formularz pozwala na podanie nieprawdziwych danych: </p> 
 
- ujemnej liczby zdobytych i straconych goli, w tych polach można dodać również literę e, jednak przy próbie dodania zawodnika pojawia się odpowiedź ze strony aplikacji, aby wprowadzić liczbę większą lub równą 0
- datę można wpisać ręcznie z klawiatury, przy czym pole roku może być nawet 6cyfrową liczbą. W przypadku wypełnienia wszystkich wymaganych pól w konfiguracji wlaśnie z takim 6cyfrowym rokiem przy próbie dodania meczu wyskakuje błąd, jednak formularz nie zwraca informacji użytkownikowi co jest nie tak w jego wypełnieniu. Devtoolsy zwracają nam informację o wystąpieniu błędu 500 - wewnętrznego błędu serwera. 
- kolor koszulki i liga powinny być moim zdaniem wybierane przez dropdown, pozostawienie wolnego pola pozwala na wpisywanie haseł nie mających odzwierciedlenia w rzeczywistości, np. znaków specjalnych
- pole czas gry pozwala na dodanie wartości większej niż 120 minut 
- pole wyboru meczu domowy/wyjazdowy nie jest oznaczone jako wymagane, a pozostawienie nie zaznaczonej żadnej z tych pozycji oznacza automatycznie mecz wyjazdowy po kliknięciu przycisku submit. 

<p align="justify"> Raport dotyczący występu i wyników zawodnika w poszczególnym meczu jest generowany na podstawie przebiegu meczu wprowadzonego za pomocą akcji „rozpocznij mecz”. Tam, w czasie rzeczywistym trwania meczu użytkownik wprowadza dane związane z występem zawodnika podczas przebiegu gry, ze wskazaniem miejsca na boisku, w którym zdarzenie wystąpiło. Funkcja ta jest jednak nieintuicyjna, dostępne w górnej części panelu przyciski nie są opisane, w związku z czym użytkownik musi kliknąć każdy z nich, celem sprawdzenia co wywołuje. Brakuje też możliwości przejścia do konkretnej minuty meczu lub przyspieszenia czasu. W obecnej formie użytkownik wprowadzając dane np. bramkarza, który w czasie trwania meczu nie ma tak częstego kontaktu z piłką jak pozostali zawodnicy, musi czekać bezczynnie aż upłynie czas do konkretnego zdarzenia z udziałem zawodnika, co wydaje się być na dłuższą metę frustrujące. Inną kwestią jest brak możliwości wyboru wszystkich możliwych zdarzeń, np. przewidzianych typowo dla bramkarza, jak obrona strzału na bramkę lub jej brak.
Mecz, który po wprowadzeniu danych nie zostanie zapisany przez użytkownika, pojawia się na stronie głównej z odnośnikiem powrotu do raportu, jednak przycisk ten nie wywołuje żadnej akcji.

 ![alt text](https://github.com/pdukat/challenge_portfolio_paulina_dukat/blob/main/validraport.JPG?raw=true)
 
 Ponadto, w tym samym momencie w zakładce issues pojawiają się dwa błędy związane z brakiem wsparcia aplikacji na niektórych przeglądarkach. 
 
 ![alt text](https://github.com/pdukat/challenge_portfolio_paulina_dukat/blob/main/issues.JPG?raw=true)

<p align="justify"> W zakładce raporty użytkownik ma możliwość przejrzeć i edytować raporty wygenerowane na podstawie poszczególnych meczów. Część danych potrzebnych do raportu jest automatycznie przetwarzana na podstawie wprowadzonych informacji z meczu, a część wymaga edycji, w postaci tekstowej, subiektywnej oceny zawodnika, do której służą proste edytory tekstu, dzięki którym można zmienić rodzaj i rozmiar czcionki, pogrubić tekst, podkreślić go, napisać kursywą, zacytować oraz wypunktować, a także cofnąć i powtórzyć ostatnie działanie. Edytor jest prosty i intuicyjny. </p> 

<p align="justify">
Aplikacja jest dostosowana do urządzeń mobilnych. Nie umożliwia jednak porównywania do siebie zawodników, co z pewnością ułatwiłoby np. podjęcie decyzji o wyborze zawodnika na daną pozycję. Do ogólnej oceny zawodnika przydałaby się funkcja robienia raportu zbiorczego, na podstawie wszystkich rozegranych meczów.</p> 
<p align="justify">
Aplikacja jest w teorii dostępna w dwóch wersjach językowych - polskiej i angielskiej, jednak w polskiej wersji nie wszystkie pola są przetłumaczone, np. przeciski "submit" i "clear", pola "Web match" i "General" w formularzu dodawania meczu, przyciski "download CSV", "print", "view columns", "filter table" w zakładce gracze, czy opisy przycisów w edytowanym raporcie. </p>   

Raport końcowy przeprowadzony za pomocą narzędzia Lighthouse ujawnił jeszcze kilka dodatkowych błędów w wyświetlaniu strony. 
[LINK DO RAPORTU](https://htmlpreview.github.io/?https://github.com/pdukat/challenge_portfolio_paulina_dukat/blob/main/scouts-test.futbolkolektyw.pl-20230116T223219.html)

# TASK 2
## Subtask 1

[PRZYPADKI TESTOWE NA PODSTAWIE USER STORY](https://docs.google.com/spreadsheets/d/1a5CcZHkxXNOqsvOUn6t_iRNmutyI7MzRRGe3EFDpcL8/edit?usp=sharing)

## Subtask 2

[PRZYPADKI TESTOWE NA PODSTAWIE WŁASNYCH DOŚWIADCZEŃ](https://docs.google.com/spreadsheets/d/1aJdtGjX23EDbuMYZd0WxBgJFTEXd28ce26LJ-b-C8TA/edit?usp=sharing)

## Subtask 3
Po co piszemy przypadki testowe?

<p align="justify"> Przypadki testowe piszemy, aby sprawdzić działanie poszczególnych funkcjonalności testowanej aplikacji. Ich tworzenie pozwala na dokładne przetestowanie modułów aplikacji i przejrzyste przedstawienie błędów, z którymi może się spotkać potencjalny użytkownik aplikacji, w celu ich naprawy. Im większe pokrycie przypadkami testowymi aplikacji, tym mniejsze prawdopodobieństwo, że któraś z ważnych funkcojalności nie będzie działała poprawnie. Za pomocą przypadków testowych sprawdzimy również, czy aplikacja jest zgodna z wymaganiami klienta.  </p>

# TASK 3
## Subtask 2

[TESTY WYKONANE WEDŁUG PLANÓW TESTÓW (TASK 2 SUBTASK 1)](https://docs.google.com/spreadsheets/d/1a5CcZHkxXNOqsvOUn6t_iRNmutyI7MzRRGe3EFDpcL8/edit?usp=sharingg)

[TESTY WYKONANE WEDŁUG PLANÓW TESTÓW (TASK 2 SUBTASK 2)](https://docs.google.com/spreadsheets/d/1aJdtGjX23EDbuMYZd0WxBgJFTEXd28ce26LJ-b-C8TA/edit?usp=sharing)

[ZBIORCZY RAPORT BŁĘDÓW](https://docs.google.com/document/d/1_U7dRavMEPdXdpny39uX4DJAGWdXxh4b-h3_sWoV1Ys/edit?usp=sharing)

## Subtask 3

[RAPORT Z WYKONANYCH TESTÓW](https://docs.google.com/document/d/1TaioT1y4r_8HDZ-dIuCcO-L8V7ME7-nrGjqKv2-8GDk/edit?usp=sharing)

## Subtask 4

[TESTY EKSPLORACYJNE](https://docs.google.com/document/d/1leQafjG6w0TSUu7WEOSyP8hLsCNmrESgDq1Onno0lvg/edit?usp=sharing)

# TASK 4
## Subtask 2

[OLX - TESTY EKSPLORACYJNE](https://docs.google.com/document/d/1CbSJ_kc7yGvm1VZ1YadWKeoKIE1_lpKVclB15Zu2AEI/edit?usp=sharing)

## Subtask 3
1. Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?

Aplikacja OLX jest platformą ogłoszeniową skupiającą przede wszystkim oferty kupna-sprzedaży produktów lub usług. Umożliwia każdemu użytkownikowi - także osobom nie prowadzącym działalności gospodarczej - zarówno sprzedaż produktów jak i ich swobodne kupno, jednocześnie pośrednicząc w tym procesie. 

2. Kto ma być użytkownikiem końcowym aplikacji?

Użytkownikiem końcowym aplikacji jest zarówno ogłoszeniodawca (np. sprzedawca czy pracodawca) jak i korzystający z ogłoszenia (jak kupujący czy korzystający z usług).

3. Czy według Ciebie aplikacja jest user friendly?

Aplikacja w ogólnym odbiorze jest przyjazna dla użytkownika, szczególnie kupującego. Szybko się ładuje, ma prosty panel do wyboru kategorii, który raczej nie pozwala się zgubić. 

4. Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? 

W mojej opinii przydałaby się możliwość wyboru podkategorii w kategorii “oddam za darmo”, żeby użytkownik mógł przejrzeć np. tylko przedmioty związane z ogrodem, nie scrollując jednocześnie nie interesujących go ofert z innych kategorii. Natomiast wśród obserwowanych ogłoszeń brakuje opcji "usuń wszystkie", umożliwiającego szybkie usunięcie wszystkich obserwowoanych ogłoszeń. 

5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?
- aplikację internetową można z łatwością przetestować tylko na jednym urządzeniu, podczas gdy aplikacja natywna wymaga korzystania z wielu urządzeń;
- testując aplikację internetową mamy możliwość korzystania z pomocy - devtoolsów, dzięki którym jesteśmy w stanie sprawdzić co powoduje błąd, testując aplikację natywną nie możemy skorzystać z takiej podpowiedzi”;
- testowanie aplikacji internetowej nie wymaga pobrania jej na urządzenie, podczas gdy aplikacji natywnej nie da się przetestować bez jej pobrania i zainstalowania 
- testowanie aplikacji internetowej zawsze wymaga dostępu do internetu, podczas gdy w wielu przypadkach aplikacji natywnych nie jest to konieczne



