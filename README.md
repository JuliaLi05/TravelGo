# TravelGo
TravelGo to statyczna strona internetowa biura podróży, stworzona przy użyciu HTML, CSS oraz biblioteki Bootstrap.

Celem projektu jest stworzenie estetycznej, intuicyjnej i responsywnej witryny prezentującej przykładową ofertę biura podróży. Strona została zaprojektowana z myślą o przejrzystej nawigacji, spójnej kolorystyce oraz dostosowaniu wyglądu do różnych rozmiarów ekranów.

## Struktura strony
Witryna składa się ze strony głównej oraz trzech podstron:
- **Strona główna (glowna.html)** – przedstawia biuro podróży TravelGo, zawiera baner powitalny, popularne kierunki wycieczek oraz krótki opis działalności.
- **Wycieczki (wycieczki.html)** – prezentuje przykładowe kierunki podróży w formie kart ze zdjęciami, opisami i przyciskami.
- **O nas (o-nas.html)** – zawiera informacje o biurze podróży, jego wartościach oraz sekcję najczęściej zadawanych pytań (FAQ).
- **Kontakt (kontakt.html)** – zawiera formularz kontaktowy umożliwiający przygotowanie wiadomości e-mail.

## Wykorzystane technologie
- **HTML5** – struktura i zawartość strony.
- **CSS3** – wygląd, układ oraz efekty wizualne.
- **Bootstrap** – gotowe komponenty i wsparcie responsywności.

## Responsywność
Strona została zaprojektowana z uwzględnieniem podejścia mobile-first. Za pomocą CSS Grid, Flexbox oraz reguł @media układ strony dostosowuje się do różnych rozmiarów ekranów.
Przykładowo karty wycieczek są wyświetlane w jednej kolumnie na telefonach, w dwóch kolumnach na tabletach, a w trzech kolumnach na większych ekranach. Dodatkowo zastosowano elastyczne rozmiary elementów oraz odpowiednie odstępy, aby zapewnić czytelność strony.

## Dostępność
W projekcie uwzględniono podstawowe zasady dostępności stron internetowych:
 - semantyczną strukturę HTML5
 - odpowiednią hierarchię nagłówków
 - atrybuty alt dla zdjęć
 - etykiety (label) przypisane do pól formularza
 - widoczne wyróżnienie elementów podczas nawigacji klawiaturą (:focus-visible)
 - kontrastową kolorystykę
 - obsługę preferencji ograniczenia animacji za pomocą prefers-reduced-motion

## Elementy interaktywne
### FAQ – najczęściej zadawane pytania
Na podstronie O nas znajduje się sekcja FAQ (Frequently Asked Questions), zawierająca najczęściej zadawane pytania i odpowiedzi dotyczące biura podróży.
Sekcja została wykonana z wykorzystaniem elementów HTML5:
- `<details>` – umożliwia rozwijanie i zwijanie odpowiedzi.
- `<summary>` – wyświetla treść pytania, którego kliknięcie powoduje rozwinięcie odpowiedzi.
Wygląd sekcji został dostosowany za pomocą CSS. Zastosowano m.in. selektor `.faq[open]`, który zmienia wygląd rozwiniętego elementu.
### Formularz kontaktowy 
FNa podstronie Kontakt znajduje się formularz kontaktowy zawierający cztery pola:
- **Imię i nazwisko** – pole tekstowe (input type="text").
- **Adres e-mail** – pole z podstawową walidacją poprawności adresu (input type="email").
- **Temat wiadomości** – pole tekstowe (input type="text").
- **Wiadomość** – wielowierszowe pole tekstowe (textarea).
Do stylizacji formularza wykorzystano klasy Bootstrapa form-control i form-label. Pola formularza zostały rozmieszczone w responsywnym układzie – na większych ekranach imię i nazwisko oraz adres e-mail znajdują się obok siebie, natomiast na urządzeniach mobilnych są wyświetlane jedno pod drugim.
#### Rozszerzane pole wiadomości
Pole Wiadomość zostało utworzone za pomocą elementu HTML <textarea>, który umożliwia wpisywanie dłuższego tekstu w wielu wierszach.
W przeciwieństwie do standardowego pola <input>, element <textarea> może być ręcznie rozszerzany przez użytkownika, jeśli pozwalają na to ustawienia przeglądarki i CSS. Dzięki temu można dostosować jego wysokość do długości wpisywanej wiadomości.
Zastosowanie tego elementu poprawia wygodę korzystania z formularza i pozwala na czytelne wprowadzanie dłuższych zapytań dotyczących wycieczek.
#### Działanie formularza
Formularz wykorzystuje mechanizm mailto:, który umożliwia otwarcie domyślnej aplikacji pocztowej użytkownika z przygotowaną wiadomością.
Wiadomość nie jest wysyłana automatycznie – użytkownik musi samodzielnie zatwierdzić jej wysłanie w programie pocztowym. Działanie formularza zależy od konfiguracji poczty na urządzeniu.
W formularzu zastosowano również atrybut required, który wymaga uzupełnienia wskazanych pól przed próbą wysłania formularza.
