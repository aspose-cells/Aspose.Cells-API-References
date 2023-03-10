---
title: classe ColumnCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 270
url: /it/python-net/aspose.cells/columncollection/
is_root: false
---
##  classe ColumnCollection
Raccolta degli oggetti [Column](/cells/it/python-net/aspose.cells/column) che rappresentano le singole colonne (impostazioni) in un foglio di lavoro.
L'oggetto Colonna rappresenta solo le impostazioni come la larghezza della colonna, gli stili, ecc. per tutta la colonna,
non ha nulla a che fare con il fatto che ci sono celle non vuote (dati) o non nella colonna corrispondente.
il "Count" di questa raccolta rappresenta solo gli oggetti Count Column di cui è stata creata un'istanza in questa raccolta,
non ha nulla a che fare con il fatto che ci sono celle non vuote (dati) o meno nel foglio di lavoro.



Il tipo ColumnCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells/columncollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [copy_to(array)](/cells/it/python-net/aspose.cells/columncollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/columncollection/index_of/#Column-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/columncollection/last_index_of/#Column) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/columncollection/last_index_of/#Column-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [get_by_index(index)](/cells/it/python-net/aspose.cells/columncollection/get_by_index/#int) | Ottiene l'oggetto colonna in base all'indice.|
| [get_column_by_index(index)](/cells/it/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Ottiene l'oggetto [Column](/cells/it/python-net/aspose.cells/column) in base alla posizione nell'elenco.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/columncollection/binary_search/#Column) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempio

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Column](/cells/it/python-net/aspose.cells/column)
