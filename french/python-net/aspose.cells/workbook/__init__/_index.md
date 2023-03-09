---
title: Workbook constructeur
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 10
url: /fr/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Remarques

Le type de format de fichier par défaut est Xlsx. Pour créer un autre type de fichier de format, veuillez utiliser Workbook(FileFormatType).
###  Exemple


Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/fr/python-net/aspose.cells/fileformattype) | Le nouveau format de fichier.|
###  Remarques

Le type de format de fichier par défaut est Excel97To2003.
###  Exemple


Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un fichier.



```python
def __init__(self, file):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| file | str | Le nom du fichier.|


##  Workbook(stream) {#io.RawIOBase}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un flux.



```python
def __init__(self, stream):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Le flux.|


##  Workbook(file, load_options) {#str-LoadOptions}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un fichier.



```python
def __init__(self, file, load_options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| file | str | Le nom du fichier.|
| load_options | [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions) | Les options de chargement|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et du flux ouvert.



```python
def __init__(self, stream, load_options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Le flux.|
| load_options | [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions) | Les options de chargement|



###  Voir également
* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
