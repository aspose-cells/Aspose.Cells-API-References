---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.


###  ritorna

[Hyperlink](/cells/it/python-net/aspose.cells/hyperlink) indice oggetto.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| cell_name | str | Cell nome.|
| total_rows | int | Numero di righe in questo intervallo di collegamenti ipertestuali.|
| total_columns | int | Numero di colonne di questo intervallo di collegamenti ipertestuali.|
| address | str | Indirizzo del collegamento ipertestuale.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.


###  ritorna

[Hyperlink](/cells/it/python-net/aspose.cells/hyperlink) indice oggetto.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| first_row | int | Prima riga dell'intervallo di collegamenti ipertestuali.|
| first_column | int | Prima colonna dell'intervallo di collegamenti ipertestuali.|
| total_rows | int | Numero di righe in questo intervallo di collegamenti ipertestuali.|
| total_columns | int | Numero di colonne di questo intervallo di collegamenti ipertestuali.|
| address | str | Indirizzo del collegamento ipertestuale.|

###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle.


###  ritorna

[Hyperlink](/cells/it/python-net/aspose.cells/hyperlink) indice oggetto.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| start_cell_name | str | La cella in alto a sinistra dell'intervallo.|
| end_cell_name | str | La cella in basso a destra dell'intervallo.|
| address | str | Indirizzo del collegamento ipertestuale.|
| text_to_display | str | Il testo da visualizzare per il collegamento ipertestuale specificato.|
| screen_tip | str | Il testo del suggerimento per il collegamento ipertestuale specificato.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Hyperlink](/cells/it/python-net/aspose.cells/hyperlink)
* classe [HyperlinkCollection](/cells/it/python-net/aspose.cells/hyperlinkcollection)
