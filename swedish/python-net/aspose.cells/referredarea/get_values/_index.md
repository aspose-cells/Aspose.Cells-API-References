---
title: get_values metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/referredarea/get_values/
is_root: false
---
##  get_values() {#}
Får cellvärden i detta område.


###  Returnerar

Om detta område är ogiltigt kommer "#REF!" att returneras;
Om detta område är en enskild cell, returnera sedan cellvärdeobjektet;
Annars returnerar du en 2D-array för alla värden i detta område.


```python
def get_values(self):
    ...
```




##  get_values(calculate_formulas) {#bool}
Får cellvärden i detta område.


###  Returnerar

Om detta område är ogiltigt kommer "#REF!" att returneras;
Om detta område är en enskild cell, returnera sedan cellvärdeobjektet;
Annars returnerar du en 2D-array för alla värden i detta område.


```python
def get_values(self, calculate_formulas):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| calculate_formulas | bool | I det här intervallet, om det finns några formler som inte har beräknats,<br/> denna flagga anger om dessa formler ska beräknas rekursivt|



###  Se även
* modul [aspose.cells](../../)
* klass [ReferredArea](/cells/sv/python-net/aspose.cells/referredarea)
