---
title: "Classe UnionRange"
linktitle: "UnionRange"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe UnionRange. Incapsula l'oggetto che rappresenta unionrange in Go."
type: docs
weight: 200
url: /it/go-cpp/unionrange/
---

## UnionRange class

Rappresenta l'intervallo di unione.

```go

type UnionRange struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetFirstRow](./getfirstrow/) | Restituisce l'indice della prima riga dell'intervallo. |
| [GetFirstColumn](./getfirstcolumn/) | Restituisce l'indice della prima colonna dell'intervallo. |
| [GetRowCount](./getrowcount/) | Ottiene il conteggio delle righe nell'intervallo. |
| [GetColumnCount](./getcolumncount/) | Ottiene il conteggio delle righe nell'intervallo. |
| [Merge](./merge/) | Combina un intervallo di celle in una singola cella. |
| [UnMerge](./unmerge/) | Separa le celle unite di questo intervallo. |
| [PutValue](./putvalue/) | Inserisce un valore nell'intervallo; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [GetValue](./getvalue/) | Ottiene e imposta i valori dell'intervallo. |
| [SetValue](./setvalue/) | Ottiene e imposta i valori dell'intervallo. |
| [GetName](./getname/) | Ottiene o imposta il nome dell'intervallo. |
| [SetName](./setname/) | Ottiene o imposta il nome dell'intervallo. |
| [GetRefersTo](./getrefersto/) | Ottiene a cosa si riferisce l'intervallo. |
| [GetHasRange](./gethasrange/) | Indica se questo ha un intervallo. |
| [GetHyperlinks](./gethyperlinks/) | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [SetStyle](./setstyle/) | Imposta lo stile dell'intervallo. |
| [ApplyStyle](./applystyle/) | Applica formati a un intero intervallo. |
| [Copy](./copy/) | Copia l'intervallo con le opzioni Incolla speciale. |
| [GetEnumerator](./getenumerator/) | Ottiene l'enumeratore per le celle in questo Range. |
| [GetCellCount](./getcellcount/) | Ottiene il conteggio totale delle celle nell'intervallo. |
| [GetRangeCount](./getrangecount/) | Ottiene il conteggio degli intervalli. |
| [GetRanges](./getranges/) | Ottiene tutti gli intervalli di unione. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Imposta i bordi di contorno attorno a un intervallo di celle. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Imposta i bordi di contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [Intersect_String](./intersect_string/) | Interseca un altro intervallo. |
| [Intersect_UnionRange](./intersect_unionrange/) | Interseca un altro intervallo. |
| [Intersect_RangeArray](./intersect_rangearray/) | Interseca un altro intervallo. |
| [Union_String](./union_string/) | Unisci un altro intervallo. |
| [Union_UnionRange](./union_unionrange/) | Unisci un altro intervallo. |
| [Union_RangeArray](./union_rangearray/) | Unisci gli intervalli. |
