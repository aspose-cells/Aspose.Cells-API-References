---
title: "UnionRange-klass"
linktitle: "UnionRange"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "UnionRange-klass. Inkapslar objektet som representerar unionrange i Go."
type: docs
weight: 200
url: /sv/go-cpp/unionrange/
---

## UnionRange class

Representerar förenad område.

```go

type UnionRange struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetFirstRow](./getfirstrow/) | Hämtar indexet för den första raden i området. |
| [GetFirstColumn](./getfirstcolumn/) | Hämtar indexet för den första kolumnen i området. |
| [GetRowCount](./getrowcount/) | Hämtar antalet rader i intervallet. |
| [GetColumnCount](./getcolumncount/) | Hämtar antalet rader i intervallet. |
| [Merge](./merge/) | Kombinerar ett cellområde till en enda cell. |
| [UnMerge](./unmerge/) | Delar upp sammanslagna celler i detta område. |
| [PutValue](./putvalue/) | Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas. |
| [GetValue](./getvalue/) | Hämtar och sätter värdena för intervallet. |
| [SetValue](./setvalue/) | Hämtar och sätter värdena för intervallet. |
| [GetName](./getname/) | Hämtar eller anger namnet på området. |
| [SetName](./setname/) | Hämtar eller anger namnet på området. |
| [GetRefersTo](./getrefersto/) | Hämtar vad området refererar till. |
| [GetHasRange](./gethasrange/) | Indikerar om detta har ett intervall. |
| [GetHyperlinks](./gethyperlinks/) | Hämtar alla hyperlänkar i intervallet. |
| [SetStyle](./setstyle/) | Anger stilen för området. |
| [ApplyStyle](./applystyle/) | Tillämpar format för ett helt område. |
| [Copy](./copy/) | Kopierar intervallet med specialklistra in-alternativ. |
| [GetEnumerator](./getenumerator/) | Hämtar enumeratorn för celler i detta Range. |
| [GetCellCount](./getcellcount/) | Hämtar det totala antalet celler i intervallet. |
| [GetRangeCount](./getrangecount/) | Hämtar antalet intervall. |
| [GetRanges](./getranges/) | Hämtar alla unionintervall. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Anger konturkanter runt ett cellområde. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Anger konturkanterna runt ett cellområde med samma kantstil och färg. |
| [Intersect_String](./intersect_string/) | Skär av ett annat intervall. |
| [Intersect_UnionRange](./intersect_unionrange/) | Skär av ett annat intervall. |
| [Intersect_RangeArray](./intersect_rangearray/) | Skär av ett annat intervall. |
| [Union_String](./union_string/) | Förenar ett annat intervall. |
| [Union_UnionRange](./union_unionrange/) | Förenar ett annat intervall. |
| [Union_RangeArray](./union_rangearray/) | Förena intervallen. |
