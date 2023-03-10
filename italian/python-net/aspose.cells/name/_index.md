---
title: classe Name
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1070
url: /it/python-net/aspose.cells/name/
is_root: false
---
##  classe Name
Rappresenta un nome definito per un intervallo di celle.



Il tipo Name espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [comment](/cells/it/python-net/aspose.cells/name/comment) | Ottiene e imposta il commento del nome.<br/> Si applica solo a Excel 2007.|
| [text](/cells/it/python-net/aspose.cells/name/text) | Ottiene il testo del nome dell'oggetto.|
| [full_text](/cells/it/python-net/aspose.cells/name/full_text) | Ottiene il testo completo del nome dell'oggetto con l'impostazione dell'ambito.|
| [refers_to](/cells/it/python-net/aspose.cells/name/refers_to) | Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con un segno di uguale.|
| [r1c1_refers_to](/cells/it/python-net/aspose.cells/name/r1c1_refers_to) | Ottiene o imposta un riferimento R1C1 di [Name](/cells/it/python-net/aspose.cells/name).|
| [is_referred](/cells/it/python-net/aspose.cells/name/is_referred) | Indica se questo nome è riferito da altre formule.|
| [is_visible](/cells/it/python-net/aspose.cells/name/is_visible) | Indica se il nome è visibile.|
| [sheet_index](/cells/it/python-net/aspose.cells/name/sheet_index) | Indica che questo nome appartiene a Cartella di lavoro o Foglio di lavoro.<br/> 0 = nome globale, altrimenti indice al foglio (a base uno)|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/it/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Ottieni il riferimento di questo nome.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/it/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Ottieni il riferimento di questo nome in base alla cella specificata.|
| [get_ranges()](/cells/it/python-net/aspose.cells/name/get_ranges/#) |Ottiene tutti gli intervalli a cui fa riferimento questo nome.|
| [get_ranges(recalculate)](/cells/it/python-net/aspose.cells/name/get_ranges/#bool) |Ottiene tutti gli intervalli a cui fa riferimento questo nome.|
| [get_range()](/cells/it/python-net/aspose.cells/name/get_range/#) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo.|
| [get_range(recalculate)](/cells/it/python-net/aspose.cells/name/get_range/#bool) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo|
| [get_range(sheet_index, row, column)](/cells/it/python-net/aspose.cells/name/get_range/#int-int-int) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo.<br/> Se il riferimento di questo nome non è assoluto, l'intervallo potrebbe essere diverso per cella diversa.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/it/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | Imposta il riferimento di questo Nome.|
| [get_referred_areas(recalculate)](/cells/it/python-net/aspose.cells/name/get_referred_areas/#bool) | Ottiene tutti i riferimenti a cui fa riferimento questo nome.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Name](/cells/it/python-net/aspose.cells/name)
