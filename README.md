#### Projekt zaliczeniowy

Zadaniem jest przygotowanie aplikacji do obsługi rezerwacji hotelowych.

Projekt jest realizowany w zespołach 1-4 osób.


Wersja `minimum` powinna obejmować:

- Cześć SQL - Zaprojektowanie struktury bazy danych, utworzenie tabel, wypełnienie przykładowymi danymi, dotyczy całego zakresu wymagań zawartych w metodach [1-10]

- Część związana z programowaniem - Utworzenie klasy `Hotel` implementującą poniższe metody [1-6]

- Przygotowanie dokumentacji bazy, krótki opis projektu.
 
Na zwiększenie oceny będzie wpływało:
- Utworzenie bezpośredniego połączenia z bazą danych, łączącego obie części projektu.
- Utworzenie dodatkowych metod klasy `Hotel` (ewentualnie samych zapytań SQL zwracających dane wyniki)
- Staranne przygotowanie kodu. Łatwość utrzymania, zgodność z dobrymi praktykami.

---

Znakiem ⭐* (metody 7-10) oznaczono zadania dodatkowe, o trudniejszym poziomie, które umożliwią wyższej oceny. Implementacja tych metod nie jest wymagana (ale w niektórych przpyadkach może okazać się niezbędna).


Klasa `Hotel` zawierająca:
- Metoda `1` tworzy nowego Klienta i dodaje do Hotelu. Metoda powinna zwrócić wygenerowany dla Klienta `clientId`.
- Metoda `2` zwraca imię i nazwisko dla użytkownika o podanym `clientId`.
- Metoda `3` zwraca liczbę niepełnoletnich klientów Hotelu.
- Metoda `4` tworzy nowy Pokój i dodaje do Hotelu. Metoda powinna zwrocić wygenerowany dla Pokoju `roomId`
- Metoda `5` zwraca powierzchnię dla pokoju o wskazanym `roomId`.
- Metoda `6` zwraca liczbę pokoi z dużym łóżkiem na wskazanym piętrze ( `floor` ).
- ⭐* Metoda `7` tworzy i zapisuje nową rezerwację dla Klienta i Pokoju o wskazanych identyfikatorach ( `clientId` oraz
roomid ) na wybrany dzień ( `date` ). Metoda powinna zwrócić wygenerowany dla Rezerwacji `reservationId`

   - Jeśli Klient o podanym `clientId` nie istnieje - wyjątek `ClientNotFoundException` powinien zostać wyrzucony
   - Jeśli Pokój o wskazanym `roomId` nie istnieje - wyjątek `RoomNotFoundException` powinien zostać wyrzucony.
   - Jeśli we wskazanym dniu Pokój jest już zarezerwowany - wyjątek `RoomReservedException` powinien zostać wyrzucony.

- ⭐* Metoda `8` zwraca informację, czy wybrany pokoj jest zarezerwowany w danym dniu. W przypadku podania `roomId`
dla którego nie istnieje Pokój - wyjątek `RoomNotFoundExcetpion` powinien zostać wyrzucony.
- ⭐* Metoda `9` zwraca liczbę niepotwierdzonych rezerwacji w danym dniu.
- ⭐* Metoda `10` zwraca unikalne identyfikatory Pokoi, które kiedykolwiek zostały zarezerwowane przez danego Klienta.

#### Do zamieszczenia na Moodle
- Katalog .zip projektu (kod sql, python i inne), w przypadku dużych zbiorów nie zamieszczamy samych danych, ale wymagany jest ich opis i wskazanie w dokumentacji,
- Plik z dokumentacją (.pdf/.md) - Opis projektu + krótka instrukcja uruchomienia i wnioski
