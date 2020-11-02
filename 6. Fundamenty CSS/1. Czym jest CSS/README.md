# Czym jest CSS?
## Przedstęp
Ta lekcja to tekstowa wersja tego co zostanie przedstawione również w trochę inny sposób w postaci wideo. CSS to na tyle ważny materiał, że postanowiłem również napisać krótki artykuł, który możesz przeanalizować na spokojnie :)

## Czym jest CSS?
**CSS** to z ang. Cascading Style Sheets czyli Kaskadowe Arkusze Stylów.

Słowo kaskada jest ciężkie do wytłumaczenia w tym kontekście także zanim zapoznam Cię z tym słowem to skupmy się na zrozumieniu pojęć “arkusze stylów”. Oczywiście czym jest kaskada powiem dokładnie później.

CSS to w skrócię język do tworzenia **arkuszy**, czyli plików z regułami które określają **styl**, czyli wygląd poszczególnych **tagów** na Twojej stronie (łatwo to teraz powiązać z ostatnimi członami nazwy ‘Style Sheets’ tzn. ‘Arkusze Stylów’). Tak więc zapamiętaj, że CSS jest odpowiedzialny za **wygląd** Twojej strony internetowej. HTML to tylko treść strony owinięta w **tagi**, które są m. in. **wykorzystywane przez CSS**.

Wykorzystywanie te polega na tym, że dobieramy (**selekcjonujemy**) tagi z pomocą tzw. **selektorów**.
```css
p {
    color :red;
}
```
Selektory należy umieścić w pliku o rozszerzeniu .css i powiązać go w pliku o rozszerzeniu .html, aby przeglądarka wiedziała gdzie szukać wyglądu strony by móc ten wygląd zobrazować (wyrenderować).**'p'** to w tym wypadku **selektor** elementów (tagów), który po prostu mówi przeglądarce aby wybrać wszystkie akapity i zastosować regułę, która znajduje się pomiędzy klamrą otwierającą **‘{‘**, a klamrą zamykającą **‘}’**. Tak więc selektor elementów działa tak, że podaje się nazwę tagu, a pomiędzy klamrami co ma się z tymi tagami stać.

Większość reguł jest tak skontruowana, że jak na nie spojrzysz to od razu wiesz co robią. Są jednak takie, które przysparzają wiele problemów początkującym twórcom stron. Nie przejmuj się bo wszystkie zostaną wyjaśnione skromnie mówiąc przeze mnie ^^

## Jak powiązać pliki reguł CSS z kodem HTML?
Spróbuj to zrobić teraz. Stwórz plik index.html, a następnie stwórz np. plik o nazwie np. test.css i powiąż go z plikiem HTML. Pamiętaj by połączenie te umieścić w nagłówku (head) strony, bo to właśnie tam przeglądarka szuka plików powiązanych (relacyjnych) do pliku html.

```html
<link rel="stylesheet" type="text/css" href="test.css">
```
Tag **link** mówi przeglądarce, że należy połączyć i wczytać plik, który określony jest przez atrybuty tagu, czyli dodatkowe informacje tzn. plik ten jest powiązany w 'rel' (relation) tzn. w relacji z tym plikiem jako 'stylesheest', czyli arkusz styli, czyli taki który zmieni wygląd strony. Typ tego arkusza to tekst css tzn. 'text/css', a znajduje się on pod nazwą 'test.css'.

Dzięki temu ‘linkowi’, czyli połączeniu z plikiem CSS przeglądarka będzie wiedzieć gdzie znajdują się **reguły** odpowiedzialne za **wygląd/styl** tagów Twojej strony internetowej. Gdy umieścisz w tym pliku css regułę którą przedstawiliśmy wyżej to wszystkie akapity staną się koloru czerwonego.

## Jakie są zalety stosowania CSS?
- Wyobraź sobie, że masz 30 akapitów na stronie, które są koloru czerwonego. Gdybyś nagle zechciał zmienić kolor tych akapitów to musiałbyś zmieniać go 30 razy. Dzięki CSS możesz to zrobić jeden raz w zewnętrznym pliku. A co jeśli miałbyś te akapity na setkach podstron? Pozostawię te pytanie bez odpowiedzi, bo się włosy jęzą na głowie ;)

- Podmieniając plik CSS można udostępnić użytkownikowi naszej strony całkowicie inny wygląd dostosowany tylko pod niego. Każdy użytkownik może mieć stronę o innym wyglądze, ale o takiej samej treści.

- Strona się szybciej wczytuje, ponieważ plik CSS wczytywany jest tylko raz po czym przechowywany jest w pamięci podręcznej (cache) i jest najczęściej spóldzielony ze wszystkimi podstronami.

- Z powyższych punktów wynika również, że oszczędzasz czas, ponieważ możesz kontrolować layout (wygląd strony) z jednego pliku mając nawet kilkaset podstron.

- Dzięki CSS możesz pokazać inną stronę użytkownikom korzystających ze smartfona, a inną korzystających z PC. Ba! możesz nawet zmienić wygląd podstrony dla osób, które chcą ją wydrukować, aby np. nie traciły kolorowego atramentu lub też ukryć menu, dla os. które zainteresowane są wydrukiem wyłącznie artykułu.

## Dlaczego po poznaniu HTML powinieneś poznać CSS?
Treść bez wyglądu nie jest atrakcyjna. Tutaj nie ma żadnej filozofii :-)

## Co oznacza słowo 'kaskada' w kontekście CSS?
Kaskada to inaczej stopniowy 'szereg'. Szereg oznacza, że coś jest ustawione w kolejności i ta kolejność ma znaczenie, ale jak to odnieść do CSS? Wyobraź sobię że nazywamy CSS następująco: Szeregowe Arkusze Stylów lub też inaczej WalcząceZeSobą Arkusze Stylów. Aby zrozumieć te słowo, należy wiedzieć, że **każda przeglądarka nadaje jakiś domyślny styl dla wszystkich tagów** oraz **style można ustawić również w tej samej linii co tag**. Najbardziej znaczące style to te, które ustawiono w linii z tagiem, po czym w arkuszach, a na końcu w przeglądarce. Jak widzisz jest tu pewnego rodzaju szereg/kolejność, która ma znaczenie przy podejmowania decyzji, który styl zostanie zastosowany. Te style tak jakby 'walczą' ze sobą o to, który zostanie zastosowany. Właśnie dlatego CSS nazywa się kaskadowym, ponieważ możemy zmienić style na kilka różnych sposobów, ale niektóre 'stopnie' zmiany są ważniejsze od innych.