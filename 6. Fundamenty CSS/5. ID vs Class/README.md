## ID vs Class
Id to identyfikator. Identyfikator musi identyfikować coś **jednoznacznie** tzn. możesz nim zidentyfikować (odróżnić) tylko **jeden** element na stronie.

Tak więc **id** stosujesz dla **unikalnego** elementu, który występuje tylko raz na całą stronę. Kiedy mówię o stronie mam na myśli jedną stronę, a nie całą witrynę. Tzn. możesz powtórzyć id="test" na różnych podstronach, ale na jednej stronie może wystąpić tylko jeden raz identyfikator o jednej wartości np. "test".

class stosujesz dla elementów, których jest wiele na stronie.

Po co tak robić? Bo selektor # wybierający identyfikatory działa szybciej niż selektor '.'

Używając "#" szukasz tylko **jednego** elementu, tak więc po znalezieniu go w drzewie (strukturze) strony, przeglądarka nie musi szukać dalej.

Natomiast, jeśli stosowałbyś "class" dla wszystkich elementów to spowolnisz wydajność swojej witryny. Nie dużo, ale jednak.

Podsumowując stosujemy:

**id**, gdy na stronie jest tylko jeden taki element np. menu górne strony

**class**, gdy na jednej stronie może być kilka elementów, które potrzebują podobnego wyglądu z poziomu CSS np. lista/paragrafy etc.