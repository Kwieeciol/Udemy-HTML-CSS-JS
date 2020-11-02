# HTML 5 vs (x)HTML vs HTML 4
Czego się uczyć jako przyszły twórca stron internetowych? Od czego zacząć swoją przygodę jako twórca stron WWW? Jak uczyć się tworzenia stron WWW? Odpowiem Ci na te pytania w poniższym artykule :)

Nie ważne jakiego typu strony internetowe będziesz robił. Nie ważne na jakiej pozycji będziesz pracował przy tworzeniu stron internetowych i tak musisz znać HTML

Najprawdopodobniej słyszałeś już o HTML. Ale czego masz się uczyć? Kiedy widzisz w jednym miejscu informacje na temat HTML, HTML 4, XHTML czy też HTML 5, już wtedy możesz nie wiedzieć od czego zacząć. Jakie są różnice?

## Czym jest HTML?

Zanim jednak przejdę do różnic: czym w skrócie jest **HTML**?

**HTML** to z ang. **H**yper **T**ext **M**arkup **L**anguage, czyli tłumacząc nieprofesjonalnie na polski **nadzwyczajny** tekstowy język znaczników.

WTF? Jak tekst może być nadzwyczajny? Tekst to przecież tylko tekst. Masz rację, ale nie do końca! Tekst bez internetu nigdy nie miał takich niezwykłych funkcjonalności jakie dały nam strony internetowe stworzone z pomocą HTML. Zabierz sobie dowolną książkę, a następnie popatrz się na spis treści. Czy kiedy zaczniesz naciskać palcami na poszczególne wpisy spisu treści to automatycznie przeniesiesz się **nadzwyczajnie** do miejsca, w którym znajduje się opisana zawartość? No, nie. Ale dzięki **hyper-link** (hiper**łączu**) z HTML jest to możliwe.

**Hiperłącza**, tabelki i inne tego typu bajery znajdują się w HTML i są definiowane, tzn. opisywane z pomocą tzw. **znaczników** (z ang. **tag**), które jak sama nazwa wskazuje **oznaczają** *zwykły* tekst pomiędzy nimi, aby stał się **nadzwyczajny**. Czyli, po prostu, nabrał jakiejś innej wartości poza byciem zwykłym tekstem.

Dla przykładu prosty kod w HTML:
```html
<b>cokolwiek</b>
```

"b" to w tym wypadku **znacznik (tag)**, który jak widzisz jest specjalnie skonstruowany - są dodane do niego znaczki "<" oraz ">", aby coś co będzie interpretowało ten kod nie pomyliło go ze zwykłym tekstem. Na dodatek znacznik zamykający ma przed sobą "/" (slash) , aby było wiadomo, kiedy nadzwyczajna interpretacja ma zostać zakończona. W tym wypadku znacznik **b** (**bold** z ang. pogrubić) pogrubia zwykły tekst pomiędzy znacznikami "cokolwiek" i na ekranie przeglądarki internetowej jest już pogrubiony. Wszystko dzięki programowi znajdującemu się w przeglądarce służącemu do interpretacji tego typu znaczników. Jak sama nazwa wskazuje przeglądarka czyli np. Chrome, Internet Explorer, Firefox służy do przeglądania i interpretacji. Nota bene w różnych przeglądarkach niektóre elementy kodu, który w przyszłości będziesz pisał mogą być minimalnie inaczej interpretowane. Czasem mogą nie zostać zinterpretowane wcale, co będzie sprawiało Ci wiele problemów. Będziesz sobie musiał oczywiście z nimi poradzić ;) Ale nie bójta się jestem tutaj z pomocą :)

Co ciekawe zabawa nie kończy się na tagach. Spróbujmy czegoś trudniejszego.

Poniżej znacznik **a** (**anchor** z ang. kotwica), który rzuca kotwicę na zwykły tekst i oczekuje podania dodatkowej informacji o tekście, aby stał się tzw. hyper-linkiem z ang. super połączeniem.

```html
<a href="http://videokurs.pl">moja strona</a> 
```

Powyżej skorzystaliśmy z atrybutu href - jest to skrót z ang. hyper reference, czyli na język polski nadzwyczajny odnośnik, tzw. link (połączenie), które odnosi się do jakiegoś miejsca. Te miejsce do którego się połączenie odnosi to “http://videokurs.pl” - jest to wartość tego atrybutu, tak jak “75kg” jest wartością dla atrybutu wagi człowieka. Zauważ, że również w tym wypadku, aby oddzielić nazwę atrybutu od wartości zostały użyte znaczki takie jak cudzysłów oraz znak równości. Nic w kodzie, ani w programowaniu nie dzieje się bez powodu. Po kliknięciu na zwyczajny tekst w tym wypadku "moja strona", który dzięki tagowi “a” stał się kotwicą oraz dzięki dodatkowej informacji z atrybutu gdzie ma prowadzić połączenie zostaniemy do tego miejsa (videokurs.pl) przeniesieni.

W przykładzie z człowiekiem, gdyby przeglądarki miały możliwość interpretacji takich tagów sytuacja wyglądałaby następująco:

```html
<czlowiek waga="75kg">Arek</czlowiek> 
```

Przeglądarki mają jednak określone jakie tagi mogą interpretować, więc powyższy przykład nie zostanie przez nie poprawnie zintepretowany. HTML określa jakie tagi / atrybuty mogą zostać użyte, aby twórcy przeglądarek mogli stworzyć odpowiednie oprogramowanie do ich interpretacji.

Takich tagów / atrybutów jest mnóstwo i większość z nich powinieneś poznać albo przynajmnej wiedzieć o ich istnieniu. Dzięki temu będziesz mógł zaglądnać do tzw. manuala (spisu ze wszystkimi tego typu informacjami), gdy będą potrzebne. Oczywiście jedną z najszybszych dróg na odnalezienie poszukiwanego tagu jest po prostu wpisanie go w wyszukiwarkę np. Google.

Z programem, który będzie interpretował specyficzny tekst, czy też różnego rodzaju dane spotkasz się w każdym języku programowania, nie tylko w HTML. W PHP zamiast tagów spotkasz się z tzw. funkcjami, które będą operować na bardziej skomplikowanych danych niż zwykły tekst. Nie będziesz w stanie znać wszystkiego na pamięć. Najważniejsze byś znał podstawy oraz w razie gdy zajdzie potrzeba, wiedział o istnieniu elementów, których nie używa się tak często. Będziesz mógł szybko je odnaleźć i przypomnieć sobie jak działają. Warto zwrócić uwagę, że często używane elementy języków powinno znać się na pamięć, gdyż usprawnia to pracę. Analogicznym przykładem jest tabliczka mnożenia w matematyce. Możesz skorzystać z kalkulatora, ale nie jest to jednak tak szybkie jak nasza pamięć.

Pewnie zastanawiasz się, dlaczego w ogóle wprowadzam Cię w HTML zamiast mówić o jego różnicach w poszczególnych wersjach. Chcę Cię nauczyć od samego początku specyficznego myślenia. Gdy poznajesz cokolwiek dotyczącego tworzenia stron WWW staraj się zrozumieć temat dogłębnie. Tłumacz sobie słówka, bo nazwy są prawie zawsze dobierane tak, by oddawały sens nazwanego elementu. s

## Jaka jest różnica między poszczególnymi wersjami HTML?

Dzięki temu, że wprowadziłem Cię do HTML, wyjaśnię Ci szybko różnicę między HTML, HTML 4, XHTML i HTML 5. Różnica jest taka, że niektóre mają więcej znaczników (HTML 5), a niektóre mniej (HTML 4). W niektórych reguły ich korzystania są bardziej rygorystyczne (XHTML), a w niektórych mniej (HTML 4).

Aktualnie najbardziej aktualnym HTML jest HTML 5, który przez to, że jest najnowszy nazywa się HTML. Śmieszne, nie? :) HTML 5 ma wiele nowych tagów; niektóre używane w poprzednich wersjach są zdeprecjonowane (z ang. deprecated) czyli przestarzałe. To oznacza, że nie powinieneś z nich już korzystać. Mimo wszystko, jeśli z nich skorzystasz to właściwie nic złego nie powinno się stać. Przeglądarki muszą sobie radzić tak, aby każdy użytkownik otrzymał treść zgodną z zamiarem twórcy strony WWW. Takie przestarzałe tagi i tak zostaną zinterpretowane, więc właściwie w większości wypadków nie masz się czym przejmować.

Jeżeli chcesz poznać HTML 5 to powinieneś znać również większość tagów, które istniały przed HTML 5. Tak więc zanim zabierzesz się za poznanie nowości z HTML 5, bez których w sumie Twoje życie jako początkującego projektanta nie zmieni się drastycznie, poznaj najpierw XHTML.

Co oznacza X przed HTML? Już wiecie co zrobie, nie? :) Tak. Dokładnie tak! Przytoczę słówko eXtended, czyli po polsku rozszerzony. Tak więc XHTML to rozszerzony HTML. Łohoho. Tak go rozszerzyli względem HTML 4, że nałożyli na niego reguły. W sumie to bardzo dobrze, bo dzięki temu w Internecie w końcu kod zaczął być pisany w bardziej elegancki sposób.

W tym kursie najpierw poznasz XHTML, a dopiero później HTML 5 (a właściwie to co dodaje od siebie ten język). Bo w sumie co za różnica skoro HTML 5 opiera się w większości na XHTML?

## BONUS: Czym jest JavaScript?
Tak naprawdę najwięcej zmienił HTML 5, bo zostały wprowadzone nowe, dosyć użyteczne tagi. Co ciekawe przeglądarki przyporządkowały do wielu z tych tagów coś co zwie się funkcjami. Można z nich skorzystać dzięki językowi JavaScript. Funkcje te, jak sama nazwa wskazuje pełnią pewnego rodzaju funkcję, czyli rolę. Dla przykładu: pozwalają w tle manipulować tym, co się dzieje na stronie. Można dynamicznie, czyli bez przeładowania strony internetowej sprawić, że coś się na stronie poruszy, np. rozwinie się schowana treść, czy też strona nabierze nowych możliwości takich jak pokazanie paska postępu, gdy wrzucamy plik na stronę internetową.

Oczywiście JavaScript istniał już dużo wcześniej, jednak funkcje, które otrzymaliśmy do tagów HTML 5 umożliwiają nawet tworzenie zaawansowanych gier przez przeglądarkę np. quakelive.com. Jako ciekawostka; na początku o stronach internetowych, w których korzystano z JavaScript mówiono, że zostały stworzone z pomocą DHTML, czyli Dynamic HTML, no bo w końcu JavaScript sprawił, że na stronach powstała dynamika czyli właśnie ruch.

UWAGA! Istnieje język programowania wysokiego poziomu Java, który nie ma nic wspólnego z JavaScript. Nie pomyl się podczas szukania informacji o JavaScript.

Podsumowując JavaScript to język stworzony specjalnie do tworzenia dynamicznych stron WWW i nie ma innego zastosowania. Wszystkie skrypty wykonywane są po stronie użytkownika odwiedzającego naszą stronę. Co to oznacza? Jak użytkownik wczyta skrypt w postaci pliku z rozszerzeniem .js to ten plik będzie u niego na komputerze. Użytkownik może go sobie przeanalizować. Można go łatwo shackować. Nie jest bezpieczny do przechowywania poufnych danych. Nie odbieraj jednak JavaScript'u jako coś złego z powodu kilku minusów. Skrypt może wykonywać się cały czas bez ponownych połączeń z serwerem i umożliwia tworzenie ruchu na stronie i responsywnego interfejsu użytkownika. 