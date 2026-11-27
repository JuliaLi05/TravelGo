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
Na podstronie Kontakt znajduje się formularz kontaktowy zawierający pola takie jak: imię i nazwisko, adres e-mail, temat wiadomości, treść wiadomości. Do stylizacji wykorzystano klasy Bootstrapa, takie jak form-control i form-label, które zapewniają spójny wygląd pól formularza. Formularz wykorzystuje mechanizm mailto:, który umożliwia otwarcie domyślnego programu pocztowego użytkownika w celu przygotowania wiadomości e-mail. Wiadomość nie jest wysyłana automatycznie – użytkownik musi samodzielnie zatwierdzić jej wysłanie w programie pocztowym. Działanie formularza zależy od konfiguracji poczty na urządzeniu.
