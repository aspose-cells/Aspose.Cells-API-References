---
title: classe Slicer
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 10
url: /it/python-net/aspose.cells.slicers/slicer/
is_root: false
---
##  classe Slicer
descrizione sommaria di Slicer Visualizza



Il tipo Slicer espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [title](/cells/it/python-net/aspose.cells.slicers/slicer/title) | Specifica il titolo dell'oggetto Slicer corrente.|
| [alternative_text](/cells/it/python-net/aspose.cells.slicers/slicer/alternative_text) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Slicer.|
| [is_printable](/cells/it/python-net/aspose.cells.slicers/slicer/is_printable) | Indica se l'oggetto slicer è stampabile.|
| [is_locked](/cells/it/python-net/aspose.cells.slicers/slicer/is_locked) | Indica se la forma dell'affettatrice è bloccata.|
| [placement](/cells/it/python-net/aspose.cells.slicers/slicer/placement) | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti.<br/> La proprietà controlla il posizionamento di un oggetto in un foglio di lavoro.|
| [locked_aspect_ratio](/cells/it/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) | Indica se bloccare le proporzioni.|
| [locked_position](/cells/it/python-net/aspose.cells.slicers/slicer/locked_position) | Indica se l'affettatrice specificata può essere spostata o ridimensionata utilizzando l'interfaccia utente.|
| [slicer_cache](/cells/it/python-net/aspose.cells.slicers/slicer/slicer_cache) |Restituisce l'oggetto SlicerCache associato all'affettatrice.|
| [parent](/cells/it/python-net/aspose.cells.slicers/slicer/parent) | Restituisce l'oggetto Worksheet che rappresenta il foglio che contiene lo slicer.|
| [style_type](/cells/it/python-net/aspose.cells.slicers/slicer/style_type) | Specificare il tipo di stile affettatrice integrato<br/> il tipo predefinito è SlicerStyleLight1|
| [name](/cells/it/python-net/aspose.cells.slicers/slicer/name) | Restituisce o imposta il nome del filtro dei dati specificato|
| [caption](/cells/it/python-net/aspose.cells.slicers/slicer/caption) | Restituisce o imposta la didascalia dell'affettatrice specificata.|
| [caption_visible](/cells/it/python-net/aspose.cells.slicers/slicer/caption_visible) | Restituisce o imposta se l'intestazione che visualizza l'affettatrice Caption è visibile<br/> il valore predefinito è vero|
| [number_of_columns](/cells/it/python-net/aspose.cells.slicers/slicer/number_of_columns) | Restituisce o imposta il numero di colonne nell'affettatrice specificata.|
| [left_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/left_pixel) | Restituisce o imposta l'offset orizzontale della forma affettatrice dalla colonna di sinistra, in pixel.|
| [top_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/top_pixel) | Restituisce o imposta l'offset verticale della forma affettatrice dalla riga superiore, in pixel.|
| [width](/cells/it/python-net/aspose.cells.slicers/slicer/width) | Restituisce o imposta la larghezza dell'affettatrice specificata, in punti.|
| [width_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/width_pixel) | Restituisce o imposta la larghezza dell'affettatrice specificata, in pixel.|
| [height](/cells/it/python-net/aspose.cells.slicers/slicer/height) | Restituisce o imposta l'altezza dell'affettatrice specificata, in punti.|
| [height_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/height_pixel) |Restituisce o imposta l'altezza dell'affettatrice specificata, in pixel.|
| [column_width_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/column_width_pixel) | Ottiene o imposta la larghezza in unità di pixel per ogni colonna dell'affettatrice.|
| [column_width](/cells/it/python-net/aspose.cells.slicers/slicer/column_width) | Restituisce o imposta la larghezza, in punti, di ogni colonna nell'affettatrice.|
| [row_height_pixel](/cells/it/python-net/aspose.cells.slicers/slicer/row_height_pixel) | Restituisce o imposta l'altezza, in pixel, di ogni riga nell'affettatrice specificata.|
| [row_height](/cells/it/python-net/aspose.cells.slicers/slicer/row_height) | Restituisce o imposta l'altezza, in punti, di ogni riga nell'affettatrice specificata.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add_pivot_connection(pivot)](/cells/it/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.PivotTable) | Aggiunge la connessione alla tabella pivot.|
| [remove_pivot_connection(pivot)](/cells/it/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.PivotTable) | Rimuove le connessioni di tabella pivot.|
| [refresh()](/cells/it/python-net/aspose.cells.slicers/slicer/refresh/#) | Aggiornamento dell'affettatrice Nel frattempo, aggiornamento e calcolo delle tabelle pivot relative.|



###  Esempi

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.slicers](..)
