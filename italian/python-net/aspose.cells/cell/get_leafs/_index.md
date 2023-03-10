---
title: metodo get_leafs
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 160
url: /it/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Ottieni tutte le celle che fanno riferimento direttamente a questa cella e devono essere aggiornate quando questa cella viene modificata.


###  ritorna

Enumeratore per enumerare tutti i dipendenti (Cell)


```python
def get_leafs(self):
    ...
```


###  Osservazioni

NOTA: questa classe è ora obsoleta. Invece,
si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo.
Questa proprietà verrà rimossa 12 mesi dopo da maggio 2022.
Aspose si scusa per gli eventuali disagi causati.

##  get_leafs(recursive) {#bool}
Ottieni tutte le celle che verranno aggiornate quando questa cella viene modificata.


###  ritorna

Enumeratore per enumerare tutti i dipendenti (Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| recursive | bool | Se restituisce quelle foglie che non fanno riferimento direttamente a questa cella<br/> ma riferimento ad altri fogli di questa cella|
###  Osservazioni

NOTA: questa classe è ora obsoleta. Invece,
si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo.
Questa proprietà verrà rimossa 12 mesi dopo da maggio 2022.
Aspose si scusa per gli eventuali disagi causati.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
