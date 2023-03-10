---
title: Workbook Konstrukteur
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 10
url: /de/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Bemerkungen

Der Standarddateiformattyp ist Xlsx. Um einen anderen Formatdateityp zu erstellen, verwenden Sie bitte Workbook (FileFormatType).
###  Beispiel


Der folgende Code zeigt, wie der Konstruktor Workbook verwendet wird, um eine neue Instanz der Klasse zu erstellen und zu initialisieren.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/de/python-net/aspose.cells/fileformattype) | Das neue Dateiformat.|
###  Bemerkungen

Der Standarddateiformattyp ist Excel97To2003.
###  Beispiel


Der folgende Code zeigt, wie der Konstruktor Workbook verwendet wird, um eine neue Instanz der Klasse zu erstellen und zu initialisieren.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook) und öffnet eine Datei.



```python
def __init__(self, file):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| file | str | Der Dateiname.|


##  Workbook(stream) {#io.RawIOBase}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook) und öffnet einen Stream.



```python
def __init__(self, stream):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Der Strom.|


##  Workbook(file, load_options) {#str-LoadOptions}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook) und öffnet eine Datei.



```python
def __init__(self, file, load_options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| file | str | Der Dateiname.|
| load_options | [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) | Die Ladeoptionen|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Initialisiert eine neue Instanz der Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook) und öffnet den Stream.



```python
def __init__(self, stream, load_options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Der Strom.|
| load_options | [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) | Die Ladeoptionen|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
