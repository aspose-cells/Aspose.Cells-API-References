---
title: index_of Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.properties/builtindocumentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Ruft den Index einer Eigenschaft nach Namen ab.


###  Kehrt zurück

Der nullbasierte Index. Negativer Wert, wenn nicht gefunden.


```python
def index_of(self, name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| name | str | Der Name der Eigenschaft ohne Berücksichtigung der Groß-/Kleinschreibung.|


##  index_of(item, index) {#DocumentProperty-int}
Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.


###  Kehrt zurück

Der nullbasierte Index des ersten Vorkommens von value innerhalb des Bereichs von Elementen in der Array-Liste, der sich von startIndex bis zum letzten Element erstreckt, falls gefunden; andernfalls -1.


```python
def index_of(self, item, index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| item | [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty) | Das Objekt, das in der Arrayliste gesucht werden soll. Der Wert kann null sein.|
| index | int | Der nullbasierte Startindex der Suche. 0 (Null) ist in einer leeren Liste gültig.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.


###  Kehrt zurück

Der nullbasierte Index des ersten Vorkommens von value innerhalb des Bereichs von Elementen in der Array-Liste, die bei startIndex beginnt und die Anzahl der Elemente enthält, falls gefunden; andernfalls -1.


```python
def index_of(self, item, index, count):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| item | [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty) | Das Objekt, das in der Arrayliste gesucht werden soll. Der Wert kann null sein.|
| index | int | Der nullbasierte Startindex der Suche. 0 (Null) ist in einer leeren Liste gültig.|
| count | int | Die Anzahl der Elemente im zu durchsuchenden Abschnitt.|



###  Siehe auch
* Modul [aspose.cells.properties](../../)
* Klasse [BuiltInDocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/builtindocumentpropertycollection)
