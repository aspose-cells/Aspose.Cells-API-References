---
title: get_value metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
Får cellvärde med given offset från det övre vänstra området i detta område.


###  Returnerar

"#REF!" om detta område är ogiltigt;
"#N/A" om den ges offset utanför detta område;
I annat fall returnerar cellvärdet vid given position.


```python
def get_value(self, row_offset, col_offset):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row_offset | int | radförskjutning från startraden i detta område|
| col_offset | int | kolumnförskjutning från startraden i detta område|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
Får cellvärde med given offset från det övre vänstra området i detta område.


###  Returnerar

"#REF!" om detta område är ogiltigt;
"#N/A" om den ges offset utanför detta område;
I annat fall returnerar cellvärdet vid given position.


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row_offset | int | radförskjutning från startraden i detta område|
| col_offset | int | kolumnförskjutning från startraden i detta område|
| calculate_formulas | bool | Beräkna det rekursivt om den angivna referensen är formel|



###  Se även
* modul [aspose.cells](../../)
* klass [ReferredArea](/cells/sv/python-net/aspose.cells/referredarea)
