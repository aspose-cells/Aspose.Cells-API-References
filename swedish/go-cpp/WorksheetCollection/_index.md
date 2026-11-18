---
title: "WorksheetCollection-klass"
linktitle: "WorksheetCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "WorksheetCollection-klass. Inkapslar objektet som representerar worksheetcollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Inkapslar en samling av <see cref="Worksheet"/>‑objekt.

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Hämtar listan över uppgiftspaneler. |
| [GetWebExtensions](./getwebextensions/) | Hämtar listan över uppgiftspaneler. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Hämtar listan över författare till trådade kommentarer. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Anger om alla anslutningar ska uppdateras vid öppning av fil i MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Anger om alla anslutningar ska uppdateras vid öppning av fil i MS Excel. |
| [CreateRange](./createrange/) | Skapar ett Range-objekt från en adress för området. |
| [CreateUnionRange](./createunionrange/) | Skapar ett Range-objekt från en adress för området. |
| [GetNames](./getnames/) | Hämtar samlingen av alla Name-objekt i kalkylbladet. |
| [Get_Int](./get_int/) | Hämtar Worksheet-elementet på det angivna indexet. |
| [Get_String](./get_string/) | Hämtar Worksheet-elementet med det angivna namnet. |
| [GetSheetByCodeName](./getsheetbycodename/) | Hämtar kalkylbladet via kodnamnet. |
| [GetActiveSheetName](./getactivesheetname/) | Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas. |
| [SetActiveSheetName](./setactivesheetname/) | Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [SortNames](./sortnames/) | Sorterar de definierade namnen. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Infoga ett kalkylblad. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Infoga ett kalkylblad. |
| [Add_SheetType](./add_sheettype/) | Lägger till ett kalkylblad i samlingen. |
| [SwapSheet](./swapsheet/) | Byter plats på de två bladen. |
| [Add](./add/) | Lägger till ett kalkylblad i samlingen. |
| [Add_String](./add_string/) | Lägger till ett kalkylblad i samlingen. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Lägger till tilläggsfunktion i arbetsboken |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Lägger till tilläggsfunktion i arbetsboken |
| [RemoveAt_String](./removeat_string/) | Tar bort elementet med ett angivet namn. |
| [RemoveAt_Int](./removeat_int/) | Tar bort elementet på ett angivet index. |
| [Clear](./clear/) | Rensa alla kalkylblad. |
| [AddCopy_String](./addcopy_string/) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [AddCopy_Int](./addcopy_int/) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Kopiera en grupp kalkylblad. |
| [GetDxfs](./getdxfs/) | Hämtar huvudposterna för differentierad formatering. |
| [GetRangeByName_String](./getrangebyname_string/) | Hämtar Range-objektet efter fördefinierat namn. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Hämtar Range efter fördefinierat namn eller tabellens namn |
| [GetNamedRanges](./getnamedranges/) | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [GetXmlMaps](./getxmlmaps/) | Hämtar och anger XML-kartor i arbetsboken. |
| [SetXmlMaps](./setxmlmaps/) | Hämtar och anger XML-kartor i arbetsboken. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla anpassade dokumentegenskaper i kalkylbladet. |
| [GetOleSize](./getolesize/) | Hämtar och anger visad storlek när arbetsboksfilen används som ett Ole-objekt. |
| [SetOleSize_Object](./setolesize_object/) | Hämtar och anger visad storlek när arbetsboksfilen används som ett Ole-objekt. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Anger visad storlek när arbetsboksfilen används som ett Ole-objekt. |
| [GetExternalLinks](./getexternallinks/) | Representerar externa länkar i en arbetsbok. |
| [GetPivotCaches](./getpivotcaches/) | Hämtar all PivotCache. |
| [GetTableStyles](./gettablestyles/) | Hämtar TableStyles-objektet. |
| [ClearPivottables](./clearpivottables/) | Rensar pivottabeller från kalkylbladet. |
| [GetRevisionLogs](./getrevisionlogs/) | Representerar revisionsloggar. |
| [RefreshPivotTables](./refreshpivottables/) | Uppdaterar alla PivotTables i Excel-filen. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Uppdaterar alla PivotTables i Excel-filen. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Representerar alla känslighetsetiketter. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
