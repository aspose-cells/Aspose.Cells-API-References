---
title: replace metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 330
url: /sv/python-net/aspose.cells/workbook/replace/
is_root: false
---
##  replace(place_holder, new_value) {#str-str}
Ersätter en cells värde med en ny sträng.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_value | str | Strängvärde att ersätta|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


##  replace(place_holder, new_value) {#str-int}
Ersätter en cells värde med ett nytt heltal.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_value | int | Heltalsvärde som ska ersättas|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


##  replace(place_holder, new_value) {#str-float}
Ersätter en cells värde med en ny dubbel.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_value | float | Dubbelt värde att byta ut|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


##  replace(bool_value, new_value) {#bool-any}
Ersätter cellernas värden med ny data.



```python
def replace(self, bool_value, new_value):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| bool_value | bool | Det booleska värdet som ska ersättas.|
| new_value | any | Nytt värde. Kan vara sträng-, heltals-, dubbel- eller DateTime-värde.|


##  replace(int_value, new_value) {#int-any}
Ersätter cellernas värden med ny data.



```python
def replace(self, int_value, new_value):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| int_value | int | Heltalsvärdet som ska ersättas.|
| new_value | any | Nytt värde. Kan vara sträng-, heltals-, dubbel- eller DateTime-värde.|


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Ersätter en cells värde med en ny strängmatris.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_values | list | Strängarray att ersätta|
| is_vertical | bool | Sant-Vertikal, Falskt-Horisontell|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Ersätter cellernas värden med en heltalsmatris.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_values | list | Heltalsmatris att ersätta|
| is_vertical | bool | Sant-Vertikal, Falskt-Horisontell|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Ersätter cellernas värden med en dubbelmatris.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_values | list | Dubbel array att byta ut|
| is_vertical | bool | Sant-Vertikal, Falskt-Horisontell|

###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_value, options) {#str-str-ReplaceOptions}
Ersätter en cells värde med en ny sträng.



```python
def replace(self, place_holder, new_value, options):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| place_holder | str | Cell platshållare|
| new_value | str | Strängvärde att ersätta|
| options | [ReplaceOptions](/cells/sv/python-net/aspose.cells/replaceoptions) | Ersätt alternativen|



###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
