# Minify & Uglify

Minify & Uglify zijn beide optimalisaties die je kan doen op het vlak van code om je website performanter te maken.

### Minify

Bij code die is geminified zijn de onnodige spaties & enters weggehaald. Hieronder zie je een voorbeeldje.

=== "Source Code"

    ```js
    function sumFromTwoNumbers(x,y) {
        let result = x + y;

        return result;
    }
    ```

=== "Minified Code"

    ```js
    function sumFromTwoNumbers(x,y) {let result = x + y;return result;}
    ```

Goed om te weten is dat we van minified code steeds terug de 'originele' code kunnen achterhalen.

![Minified code leesbaarder maken m.b.h.v Chrome Dev Tools](../_resources/images/screenshot-20-09-2021at-18.19.10.gif)

### Uglify

Bij code die is 'geuglified' zijn namen van variabelen en functies, in sommige gevallen ook hele delen code, veranderd of herschreven om de code korter \(en de file dus kleiner qua grootte\) te maken.

=== "Source Code"

    ```js
    function sumFromTwoNumbers(x,y) {
        let result = x + y;

        return result;
    }
    ```

=== "Uglified Code"

    ```js
    function s(r,u){return r+u}
    ```

!!! warning "LET OP"
    Uglify'en is een destructieve actie, de originele code kan niet meer achterhaald worden. Er is bij uglify'en ook meer kans tot de introductie van bugs...

!!! info "Automatisatie"
    Later zal je zien dat er automatische processen zijn die er voor zorgen dat de code die jij schrijft automatisch wordt geminified/uglified alvorens ze ergens online komt.
