# Specificità nei selettori CSS
La specificità è un modo per determinare quale stile CSS verrà applicato a un elemento HTML in presenza di più stili in conflitto. La specificità di un selettore può essere calcolata come un valore a quattro cifre, dove ogni cifra rappresenta il numero di vari tipi di selettore utilizzati nel selettore. Il selettore più specifico vince quando più selettori prendono di mira lo stesso elemento HTML.

Qui c'è una lista di selettori con il loro grado di specificità:

1. ``ul li {}``
> Specificity: 002

2. ``ul > li {}``
> Specificity: 012

3. ``ody > #main.mobile a:hover {}``
> Specificity: 013

4. ``div p > span {}``
> Specificity: 012

5. ``.users .name {}``
> Specificity: 002

6. ``[href$='.pdf'] {}``
> Specificity: 010

7. ``:hover {}``
> Specificity: 001

8. ``div .name {}``
> Specificity: 010

9. ``a[href$='.pdf'] {}``
> Specificity: 011

10. ``.pictures img:hover {}``
> Specificity: 011

11. ``.news.breaking.featured {}``
> Specificity: 003

12. ``.user #name {}``
> Specificity: 011

13. ``#name span {}``
> Specificity: 011

14. ``nav#nav > li:hover {}``
> Specificity: 012

15. ``li:nth-child(2n+1):hover {}``
> Specificity: 012