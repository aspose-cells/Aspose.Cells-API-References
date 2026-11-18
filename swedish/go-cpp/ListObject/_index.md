---
title: "ListObject-klass"
linktitle: "ListObject"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ListObject-klass. Inkapslar objektet som representerar listobject i Go."
type: docs
weight: 200
url: /sv/go-cpp/listobject/
---

## ListObject class

Representerar en tabell i ett kalkylblad.

```go

type ListObject struct  {
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
| [GetStartRow](./getstartrow/) | Hämtar startraden för intervallet. |
| [GetStartColumn](./getstartcolumn/) | Hämtar startkolumnen för intervallet. |
| [GetEndRow](./getendrow/) | Hämtar slutraden för intervallet. |
| [GetEndColumn](./getendcolumn/) | Hämtar slutkolumnen för intervallet. |
| [GetListColumns](./getlistcolumns/) | Hämtar ListColumn-listan för den här tabellen. |
| [Resize](./resize/) | Ändra storlek på intervallet för listobjektet. |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Sätt värdet i cellen. |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Sätt värdet i cellen. |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Sätt formeln i cellen i tabellen. |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Sätt formeln i cellen i tabellen. |
| [GetShowHeaderRow](./getshowheaderrow/) | Hämtar och anger om den här tabellen visar rubrikrad. |
| [SetShowHeaderRow](./setshowheaderrow/) | Hämtar och anger om den här tabellen visar rubrikrad. |
| [GetShowTotals](./getshowtotals/) | Hämtar och anger om den här TAble visar totalsrad. |
| [SetShowTotals](./setshowtotals/) | Hämtar och anger om den här TAble visar totalsrad. |
| [GetDataRange](./getdatarange/) | Hämtar dataintervallet för tabellen. |
| [UpdateColumnName](./updatecolumnname/) | Uppdaterar alla listkolumners namn till cellerna i tabellen. |
| [GetQueryTable](./getquerytable/) | Hämtar den länkade QueryTable. |
| [GetDataSourceType](./getdatasourcetype/) | Hämtar datakälltyp för tabellen. |
| [GetHasAutoFilter](./gethasautofilter/) | Anger om autofilter är tillämpat på den här tabellen. |
| [SetHasAutoFilter](./sethasautofilter/) | Anger om autofilter är tillämpat på den här tabellen. |
| [RemoveAutoFilter](./removeautofilter/) | Tar bort autofilter som är tillämpat på den här tabellen. |
| [GetAutoFilter](./getautofilter/) | Hämtar autofilter för den här tabellen. |
| [GetDisplayName](./getdisplayname/) | Hämtar och anger visningsnamnet för tabellen. |
| [SetDisplayName](./setdisplayname/) | Hämtar och anger visningsnamnet för tabellen. |
| [GetComment](./getcomment/) | Hämtar och anger kommentaren för tabellen. |
| [SetComment](./setcomment/) | Hämtar och anger kommentaren för tabellen. |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Indikerar om den första kolumnen i tabellen är den tillämpade stilen. |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Indikerar om den första kolumnen i tabellen är den tillämpade stilen. |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Indikerar om den sista kolumnen i tabellen är den tillämpade stilen. |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Indikerar om den sista kolumnen i tabellen är den tillämpade stilen. |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Indikerar om radrandig formatering är tillämpad. |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Indikerar om radrandig formatering är tillämpad. |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Indikerar om kolumnrandig formatering är tillämpad. |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Indikerar om kolumnrandig formatering är tillämpad. |
| [ApplyStyleToRange](./applystyletorange/) | Applicera tabellstilen på området. |
| [ConvertToRange](./converttorange/) | Konvertera tabellen till ett område. |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | Konvertera tabellen till ett område. |
| [GetTableStyleType](./gettablestyletype/) | Hämtar och den inbyggda tabellstilen. |
| [SetTableStyleType](./settablestyletype/) | Hämtar och den inbyggda tabellstilen. |
| [GetTableStyleName](./gettablestylename/) | Hämtar och anger tabellstilens namn. |
| [SetTableStyleName](./settablestylename/) | Hämtar och anger tabellstilens namn. |
| [GetXmlMap](./getxmlmap/) | Hämtar en XmlMap som används för den här listan. |
| [GetAlternativeText](./getalternativetext/) | Hämtar och anger den alternativa texten. |
| [SetAlternativeText](./setalternativetext/) | Hämtar och anger den alternativa texten. |
| [GetAlternativeDescription](./getalternativedescription/) | Hämtar och anger den alternativa beskrivningen. |
| [SetAlternativeDescription](./setalternativedescription/) | Hämtar och anger den alternativa beskrivningen. |
