---
title: classe CustomDocumentPropertyCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  classe CustomDocumentPropertyCollection
Una raccolta di proprietà del documento personalizzate.



**Eredità:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/documentpropertycollection)



Il tipo CustomDocumentPropertyCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [capacity](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [index_of(name)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Ottiene l'indice di una proprietà in base al nome.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [copy_to(array)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) | Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [add(name, value)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Crea una nuova proprietà del documento personalizzata di**PropertyType.String** tipo di dati.|
| [add(name, value)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Crea una nuova proprietà del documento personalizzata di**TipoProprietà.Numero** tipo di dati.|
| [add(name, value)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Crea una nuova proprietà del documento personalizzata di**PropertyType.DateTime** tipo di dati.|
| [add(name, value)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Crea una nuova proprietà del documento personalizzata di**PropertyType.Boolean** tipo di dati.|
| [add(name, value)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Crea una nuova proprietà del documento personalizzata di**PropertyType.Float** tipo di dati.|
| [binary_search(item)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|
| [add_link_to_content(name, source)](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Crea una nuova proprietà del documento personalizzata che si collega al contenuto.|
| [update_linked_property_value()](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) | Aggiorna il valore della proprietà del documento personalizzato che collega al contenuto.|
| [update_linked_range()](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Aggiorna il valore della proprietà del documento personalizzato all'intervallo collegato.|



###  Osservazioni

Ogni oggetto [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) rappresenta una proprietà personalizzata di un documento contenitore.

###  Esempio

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Guarda anche
* modulo [aspose.cells.properties](..)
* classe [CustomDocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection)
* classe [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty)
* classe [DocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/documentpropertycollection)
