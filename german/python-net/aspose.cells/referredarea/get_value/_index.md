---
title: get_value Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
Ruft den Zellenwert mit dem angegebenen Offset von der linken oberen Ecke dieses Bereichs ab.


###  Kehrt zurück

„#REF!“ wenn dieser Bereich ungültig ist;
"#N/A", wenn ein Offset außerhalb dieses Bereichs angegeben wird;
Andernfalls den Zellenwert an der angegebenen Position zurückgeben.


```python
def get_value(self, row_offset, col_offset):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row_offset | int | Zeilenversatz von der Startzeile dieses Bereichs|
| col_offset | int |Spaltenversatz von der Startzeile dieses Bereichs|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
Ruft den Zellenwert mit dem angegebenen Offset von der linken oberen Ecke dieses Bereichs ab.


###  Kehrt zurück

„#REF!“ wenn dieser Bereich ungültig ist;
"#N/A", wenn ein Offset außerhalb dieses Bereichs angegeben wird;
Andernfalls den Zellenwert an der angegebenen Position zurückgeben.


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row_offset | int | Zeilenversatz von der Startzeile dieses Bereichs|
| col_offset | int |Spaltenversatz von der Startzeile dieses Bereichs|
| calculate_formulas | bool | Ob es rekursiv berechnet wird, wenn die angegebene Referenz eine Formel ist|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [ReferredArea](/cells/de/python-net/aspose.cells/referredarea)
