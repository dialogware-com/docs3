[Programowanie imperatywne oraz deklaratywne | Codenga](https://codenga.pl/artykuly/poradniki/programowanie-imperatywne-oraz-deklaratywne)

> # Programowanie imperatywne oraz deklaratywne
>
> W programowaniu imperatywnym skupiamy się na krokach prowadzących do rozwiązania problemu. Z kolei w programowaniu deklaratywnym bardziej interesuje nas rezultat niż sposób rozwiązania danego problemu.
>
> ### O co tutaj chodzi?
>
> Programowanie wymaga właściwego podejścia. Każdy program jest inny. Każdy program trzeba “rozgryźć” we właściwy sposób.
>
> Dlatego istnieją tzw. paradygmaty programowania. To nic innego jak pewien styl pisania kodu. W tym artykule przyjrzymy się uważnie dwóm głównym paradygmatom programowania.
>
> ### Programowanie imperatywne
>
> Paradygmat imperatywny można opisać tak: “mówimy jak komputer ma wykonać daną rzecz”. Czyli skupiamy się na poszczególnych krokach, które prowadzą do rozwiązania problemu.
>
> Możesz sobie wyobrazić program napisany imperatywnie jako ciąg instrukcji. Takie podejście jest dla nas zrozumiałe. Łatwo jest prześledzić wszystkie kroki wykonywane przez program. Z tego powodu programowanie imperatywne jest zazwyczaj pierwszym paradygmatem, na który napotykają początkujący programiści.
>
> ### Przykład
>
> Najlepiej będzie to zilustrować przykładem opartym na realnym kodzie.. Mamy prostą tablicę z wartościami liczbowymi i chcemy z niej odrzucić wartości równe 1. Popatrz na kod w języku JavaScript:
>
>     let arr = [1, 2, 3];
>     let filteredArr = [];
>     for (let i = 0; i < arr.length; i++) {
>         let v = arr[i];
>         if (v != 1) {
>           filteredArr.push(v);
>         }
>     }
>     console.log(filteredArr);
>
>
> To oczywiście przykład kodu napisanego imperatywnie. Zauważ, że musimy krok po kroku dokładnie opisać wszystkie instrukcje jaki mają być wykonane:
>
> 1.  Stwórz nową, pustą tablicę o nazwie **filteredArr**.
> 2.  Za pomocą pętli przetwórz tablicę **arr**. Zakończ pętlę jak wyczerpią się wszystkie wartości w tablicy.
> 3.  W pętli stwórz zmienną **v**, która przechowuje pojedyncze wartości z tablicy.
> 4.  Za pomocą instrukcji warunkowej sprawdź wartość zmiennej **v**.
> 5.  Jeśli wartość v jest inna niż 1, to wstaw taką wartość do tablicy **filteredArr**.
>
> Po prostu tutaj “prowadzimy komputer za rękę” i dokładnie mu wskazujemy co ma wykonać w każdym kroku.
>
> ### Programowanie deklaratywne
>
> Paradygmat deklaratywny można opisać tak: “mówimy komputerowi co ma dla nas zrobić”. Ważny jest dla nas wynik jaki uzyskamy - nie wnikamy w jaki sposób komputer ten wynik. osiągnie.
>
> Taki styl programowania pozwala skupić się więc na celu. Na tym, co chcemy osiągnąć. Mniej ważne są tutaj kroki, które do tego celu prowadzą.
>
> ### Przykład
>
> Spróbujemy teraz rozwiązać znany nam już problem w sposób bardziej deklaratywny:
>
>     let arr = [1, 2, 3];
>     function checkValue(v) {
>       return v != 1;
>     }
>     console.log(arr.filter(checkValue));
