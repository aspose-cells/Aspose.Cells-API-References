---
title: Workbook konstruktör
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Anmärkningar

Standardfilformatstypen är Xlsx. För att skapa annan filtyp, använd Workbook(FileFormatType).
###  Exempel


Följande kod visar hur man använder konstruktorn Workbook för att skapa och initiera en ny instans av klassen.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/sv/python-net/aspose.cells/fileformattype) | Det nya filformatet.|
###  Anmärkningar

Standardfilformatet är Excel97To2003.
###  Exempel


Följande kod visar hur man använder konstruktorn Workbook för att skapa och initiera en ny instans av klassen.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook) och öppnar en fil.



```python
def __init__(self, file):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| file | str | Filnamnet.|


##  Workbook(stream) {#io.RawIOBase}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook) och öppnar en ström.



```python
def __init__(self, stream):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Strömmen.|


##  Workbook(file, load_options) {#str-LoadOptions}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook) och öppnar en fil.



```python
def __init__(self, file, load_options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| file | str | Filnamnet.|
| load_options | [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions) | Lastalternativen|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Initierar en ny instans av klassen [Workbook](/cells/sv/python-net/aspose.cells/workbook) och öppen ström.



```python
def __init__(self, stream, load_options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Strömmen.|
| load_options | [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions) | Lastalternativen|



###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
