---
title: "AutoFilter-klass"
linktitle: "AutoFilter"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AutoFilter-klass. Inkapslar objektet som representerar autofilter i Go."
type: docs
weight: 200
url: /sv/go-cpp/autofilter/
---

## AutoFilter class

Representerar autofilter för det angivna kalkylbladet.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Hämtar datasorteringen. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Anger intervallet som den specificerade AutoFilter gäller för. |
| [GetCellArea](./getcellarea/) | Hämtar CellArea där denna AutoFilter gäller. |
| [GetCellArea_Bool](./getcellarea_bool/) | Hämtar Aspose.Cells.CellArea där den specificerade AutoFilter gäller. |
| [GetRange](./getrange/) | Representerar intervallet som den specificerade AutoFilter gäller för. |
| [SetRange_String](./setrange_string/) | Representerar intervallet som den specificerade AutoFilter gäller för. |
| [AddFilter](./addfilter/) | Lägger till ett filter för en filterkolumn. |
| [AddDateFilter](./adddatefilter/) | Lägger till ett datumfilter. |
| [RemoveDateFilter](./removedatefilter/) | Tar bort ett datumfilter. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Tar bort ett filter för en filterkolumn. |
| [Filter](./filter/) | Filtrerar en lista med specificerade kriterier. |
| [FilterTop10](./filtertop10/) | Filtrera de 10 bästa objekten i listan |
| [Dynamic_Filter](./dynamic_filter/) | Lägger till ett dynamiskt filter. |
| [AddFontColorFilter](./addfontcolorfilter/) | Lägger till ett teckensnittsfärgsfilter. |
| [AddFillColorFilter](./addfillcolorfilter/) | Lägger till ett fyllnadsfärgsfilter. |
| [AddIconFilter](./addiconfilter/) | Lägger till ett ikonfilter. |
| [MatchBlanks](./matchblanks/) | Matcha alla tomma celler i listan. |
| [MatchNonBlanks](./matchnonblanks/) | Matcha alla icke-tomma celler i listan. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filtrerar en lista med ett anpassat kriterium. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filtrerar en lista med anpassade kriterier. |
| [ShowAll](./showall/) | Visa alla rader. |
| [RemoveFilter_Int](./removefilter_int/) | Ta bort det specifika filtret. |
| [Refresh](./refresh/) | Uppdatera autofilter för att dölja eller visa raderna. |
| [Refresh_Bool](./refresh_bool/) | Hämtar alla dolda raders index. |
| [GetShowFilterButton](./getshowfilterbutton/) | Anger om AutoFilter-knappen för den här kolumnen är synlig. |
| [SetShowFilterButton](./setshowfilterbutton/) | Anger om AutoFilter-knappen för den här kolumnen är synlig. |
| [GetFilterColumns](./getfiltercolumns/) | Hämtar samlingen av filterkolumnerna. |
