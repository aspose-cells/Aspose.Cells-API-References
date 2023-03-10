---
title: Workbook costruttore
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 10
url: /it/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Osservazioni

Il tipo di formato file predefinito è Xlsx. Per creare un altro tipo di file di formato, utilizzare Workbook(FileFormatType).
###  Esempio


Il codice seguente mostra come usare il costruttore Workbook per creare e inizializzare una nuova istanza della classe.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/it/python-net/aspose.cells/fileformattype) | Il nuovo formato file.|
###  Osservazioni

Il tipo di formato file predefinito è Excel97To2003.
###  Esempio


Il codice seguente mostra come usare il costruttore Workbook per creare e inizializzare una nuova istanza della classe.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un file.



```python
def __init__(self, file):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| file | str | Il nome del file.|


##  Workbook(stream) {#io.RawIOBase}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un flusso.



```python
def __init__(self, stream):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| stream | io.RawIOBase | Il flusso.|


##  Workbook(file, load_options) {#str-LoadOptions}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un file.



```python
def __init__(self, file, load_options):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| file | str | Il nome del file.|
| load_options | [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions) | Le opzioni di caricamento|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre il flusso.



```python
def __init__(self, stream, load_options):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| stream | io.RawIOBase | Il flusso.|
| load_options | [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions) | Le opzioni di caricamento|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
