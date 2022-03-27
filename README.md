# Projekt część I - Ruby

## Organizacja projektu
* należy pracować w grupach trzy- lub czteroosobowych
* może istnieć jedna grupa czteroosobowa
* składy grup należy przesłać do mnie w wiadomości prywatnej na MS Teams
* osoby które nie prześlą składów grup do 28/03 20:00 zostaną przydzielono do grup losowo
* skład grup nie może zmieniać się pomiędzy etapami projektów
* wkład wszystkich członków zespołów liczony na przestrzeni semestru powinien być równy (wkład liczony jest na podstawie liczby commitów i/lub liczby linii kodu)

## Język Ruby
Istnieje wiele kursów online pozwalających na zapoznanie się z językiem Ruby. Przykładowe to [Ruby tutorial na tutorialspoint.com](https://www.tutorialspoint.com/ruby/index.htm) lub [Ruby w 20 minut](https://www.ruby-lang.org/pl/documentation/quickstart/). Wraz z pogłębianiem swojej wiedzy należy samodzielnie poszukiwać źródeł najbardziej odpowiednich dla siebie.

## Ruby a testy
Najbardziej popularną biblioteką służącą do pisania testów w Ruby jest biblioteka RSpec. Zapoznać się można z nią przykładowo [tutaj](https://semaphoreci.com/community/tutorials/getting-started-with-rspec).

## Zadania
1. Klasa Employee (2 punkty)
   * należy zaimplementować klasę reprezentującą pracownika
   * klasa ta ma jako parametry konstruktora przyjmować `name`, `surname`, `id`
   * parametry `name`, `surname`, `id` mają być parametrami tylko do odczytu `attr_reader`
   * dodatkowo klasa ma mieć następujące parametry dostępne zarówno do odczytu jak i zapisu: `company`, `position`, `salary`
2. Klasa EmployeeDirectory (2 punkty)
   * klasa ma przechowywać zbór obiektów klasy `Employee`
   * klasa ma mieć metodę `with_salary_over(salary)` zwracającą listę pracowników których wynagrodzenia są wyższe niż wartość przekazana jako argument metody
   * klasa ma mieć metodę `salaries_sorted` zwracającą listę pracowników posortowanych wg ich wynagrodzenia, zaczynając od najnliższego wynagrodzenia
   * klasa ma mieć metodę `working_for(company)` zwracającą listę osób pracujących dla firmy przekazanej jako argument metody (wielkość liter nie powinna mieć znaczenia)
   * klasa ma mieć metodę `with_position(position)` zwracającą listę osób pracujących na stanowisku przekazanym jako argument metody (wielkość liter nie powinna mieć znaczenia)
3. Test jednostkowe (4 punkty)
   * należy napisać testy jednostkowo z użyciem `RSpec` testujące wszystkie funkcjonalności
   * należy,wraz z kodem, przesłać do repozytorium raport pokrycia kodu testami
   * pokrycie nie może być mniejsze niż **80%**