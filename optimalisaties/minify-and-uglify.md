# Minify & Uglify

{% tabs %}
{% tab title="Uglified Code" %}
```text
   let result = x + y;
   
   return result;
} 
```
{% endtab %}
{% endtabs %}

Minify & Uglify zijn beide optimalisaties die je kan doen op het vlak van code om je website performanter te maken.

### Minify

Bij code die is geminified zijn de onnodige spaties & enters weggehaald. Hieronder zie je een voorbeeldje.

{% tabs %}
{% tab title="Source Code" %}
```text
function sumFromTwoNumbers(x,y) {
   let result = x + y;
   
   return result;
} 
```
{% endtab %}

{% tab title="Minified Code" %}
```text
function sumFromTwoNumbers(x,y) {let result = x + y;return result;} 
```
{% endtab %}
{% endtabs %}

Goed om te weten is dat we van minified code steeds terug de 'originele' code kunnen achterhalen.

![Minified code leesbaarder maken m.b.h.v Chrome Dev Tools](../.gitbook/assets/screenshot-20-09-2021at-18.19.10.gif)

### Uglify

Bij code die is 'geuglified' zijn namen van variabelen en functies, in sommige gevallen ook hele delen code, veranderd of herschreven om de code korter \(en de file dus kleiner qua grootte\) te maken.

{% tabs %}
{% tab title="Source Code" %}
```text
function sumFromTwoNumbers(x,y) {
   let result = x + y;
   
   return result;
} 
```
{% endtab %}

{% tab title="Uglified Code" %}
```text
function s(r,u){return r+u}
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
Uglify'en is een destructieve actie, de originele code kan niet meer achterhaald worden. Er is bij uglify'en ook meer kans tot de introductie van bugs...
{% endhint %}

{% hint style="info" %}
Later zal je zien dat er automatische processen zijn die er voor zorgen dat de code die jij schrijft automatisch wordt geminified/uglified alvorens ze ergens online komt.
{% endhint %}



{% page-ref page="plaatsing-resources.md" %}



