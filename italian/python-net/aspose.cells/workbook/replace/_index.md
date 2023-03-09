---
title: metodo replace
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 330
url: /it/python-net/aspose.cells/workbook/replace/
is_root: false
---
##  replace(place_holder, new_value) {#str-str}
Sostituisce il valore di una cella con una nuova stringa.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_value | str | Valore stringa da sostituire|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


##  replace(place_holder, new_value) {#str-int}
Sostituisce il valore di una cella con un nuovo numero intero.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_value | int | Valore intero da sostituire|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


##  replace(place_holder, new_value) {#str-float}
Sostituisce il valore di una cella con un nuovo double.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_value | float | Valore doppio da sostituire|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


##  replace(bool_value, new_value) {#bool-any}
Sostituisce i valori delle celle con nuovi dati.



```python
def replace(self, bool_value, new_value):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| bool_value | bool | Il valore booleano da sostituire.|
| new_value | any | Nuovo valore. Può essere una stringa, un numero intero, un valore double o DateTime.|


##  replace(int_value, new_value) {#int-any}
Sostituisce i valori delle celle con nuovi dati.



```python
def replace(self, int_value, new_value):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| int_value | int | Il valore intero da sostituire.|
| new_value | any | Nuovo valore. Può essere una stringa, un numero intero, un valore double o DateTime.|


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Sostituisce il valore di una cella con un nuovo array di stringhe.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_values | list | Matrice di stringhe da sostituire|
| is_vertical | bool | Vero-Verticale, Falso-Orizzontale|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Sostituisce i valori delle celle con un array intero.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_values | list | Matrice intera da sostituire|
| is_vertical | bool | Vero-Verticale, Falso-Orizzontale|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Sostituisce i valori delle celle con un doppio array.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_values | list | Doppio array da sostituire|
| is_vertical | bool | Vero-Verticale, Falso-Orizzontale|

###  Esempi

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_value, options) {#str-str-ReplaceOptions}
Sostituisce il valore di una cella con una nuova stringa.



```python
def replace(self, place_holder, new_value, options):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| place_holder | str | Cell segnaposto|
| new_value | str | Valore stringa da sostituire|
| options | [ReplaceOptions](/cells/it/python-net/aspose.cells/replaceoptions) | Le opzioni di sostituzione|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
