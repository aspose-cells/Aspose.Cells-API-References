---
title: "DataSorter-klass"
linktitle: "DataSorter"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DataSorter-klass. Inkapslar objektet som representerar datasorter i Go."
type: docs
weight: 200
url: /sv/go-cpp/datasorter/
---

## DataSorter class

Sammanfattande beskrivning för DataSorter.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | Hämtar nyckellistan för datasortering. |
| [Clear](./clear/) | Rensa alla inställningar. |
| [GetHasHeaders](./gethasheaders/) | Representerar om området har rubriker. |
| [SetHasHeaders](./sethasheaders/) | Representerar om området har rubriker. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | Lägger till sorterat kolumnindex och sorteringsordning. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [AddColorKey](./addcolorkey/) | Lägger till färgsorteringsnyckel. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [GetKey1](./getkey1/) | Representerar första sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [SetKey1](./setkey1/) | Representerar första sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [GetOrder1](./getorder1/) | Representerar sorteringsordning för den första nyckeln. |
| [SetOrder1](./setorder1/) | Representerar sorteringsordning för den första nyckeln. |
| [GetKey2](./getkey2/) | Representerar andra sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [SetKey2](./setkey2/) | Representerar andra sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [GetOrder2](./getorder2/) | Representerar sorteringsordning för den andra nyckeln. |
| [SetOrder2](./setorder2/) | Representerar sorteringsordning för den andra nyckeln. |
| [GetKey3](./getkey3/) | Representerar tredje sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [SetKey3](./setkey3/) | Representerar tredje sorterade kolumnindex (absolut position, kolumn A är 0, B är 1, ...). |
| [GetOrder3](./getorder3/) | Representerar sorteringsordning för den tredje nyckeln. |
| [SetOrder3](./setorder3/) | Representerar sorteringsordning för den tredje nyckeln. |
| [GetSortLeftToRight](./getsortlefttoright/) | True betyder att sorteringsriktningen är från vänster till höger. False betyder att sorteringsriktningen är från topp till botten. Standardvärdet är false. |
| [SetSortLeftToRight](./setsortlefttoright/) | True betyder att sorteringsriktningen är från vänster till höger. False betyder att sorteringsriktningen är från topp till botten. Standardvärdet är false. |
| [GetCaseSensitive](./getcasesensitive/) | Hämtar och anger om skiftlägeskänslighet ska användas vid jämförelse av strängar. |
| [SetCaseSensitive](./setcasesensitive/) | Hämtar och anger om skiftlägeskänslighet ska användas vid jämförelse av strängar. |
| [GetSortAsNumber](./getsortasnumber/) | Indikerar om sortering ska göras på allt som ser ut som ett tal. |
| [SetSortAsNumber](./setsortasnumber/) | Indikerar om sortering ska göras på allt som ser ut som ett tal. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Sorterar data i området. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | Sortera data i området. |
| [Sort](./sort/) | Sortera data i intervallet. |
