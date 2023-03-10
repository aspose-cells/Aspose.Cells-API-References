---
title: metodo import_xml
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 220
url: /it/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Importa/aggiorna un file di dati XML nella cartella di lavoro.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| url | str | l'URL/percorso del file xml.|
| sheet_name | str | il nome del foglio di destinazione.|
| row | int | la riga di destinazione|
| col | int | la colonna di destinazione|

###  Esempio

Il codice seguente importa i dati XML nel foglio di lavoro "Foglio 1" in Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Importa/aggiorna un file di dati XML nella cartella di lavoro.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| stream | io.RawIOBase | il flusso di file xml.|
| sheet_name | str | il nome del foglio di destinazione.|
| row | int | la riga di destinazione.|
| col | int | la colonna di destinazione.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
