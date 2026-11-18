---
title: "ImportTableOptions-klass"
linktitle: "ImportTableOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ImportTableOptions-klass. Inkapslar objektet som representerar importtableoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/importtableoptions/
---

## ImportTableOptions class

Representerar alternativen för att importera data till celler.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Skapar standardalternativen för import. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Anger om stilen för rutnätsvyn ska tillämpas på celler. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Anger om stilen för rutnätsvyn ska tillämpas på celler. |
| [GetConvertNumericData](./getconvertnumericdata/) | Hämtar eller anger ett värde som indikerar om strängvärdet ska konverteras till numeriskt eller datumvärde. |
| [SetConvertNumericData](./setconvertnumericdata/) | Hämtar eller anger ett värde som indikerar om strängvärdet ska konverteras till numeriskt eller datumvärde. |
| [GetInsertRows](./getinsertrows/) | Anger om nya rader ska läggas till för import av dataposter. |
| [SetInsertRows](./setinsertrows/) | Anger om nya rader ska läggas till för import av dataposter. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Anger om den första raden ska flyttas nedåt vid infogning av rader. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Anger om den första raden ska flyttas nedåt vid infogning av rader. |
| [IsFieldNameShown](./isfieldnameshown/) | Anger om fältnamnet ska importeras. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Anger om fältnamnet ska importeras. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Anger om rubrik ska exporteras som fältnamn. |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Anger om rubrik ska exporteras som fältnamn. |
| [GetDateFormat](./getdateformat/) | Hämtar eller anger datumformatsträng för celler med importerade datum/tidsvärden. |
| [SetDateFormat](./setdateformat/) | Hämtar eller anger datumformatsträng för celler med importerade datum/tidsvärden. |
| [GetNumberFormats](./getnumberformats/) | Hämtar eller anger talformaten. |
| [SetNumberFormats](./setnumberformats/) | Hämtar eller anger talformaten. |
| [GetStyles](./getstyles/) | Hämtar och anger stilarna för varje kolumn i tabellen. |
| [SetStyles](./setstyles/) | Hämtar och anger stilarna för varje kolumn i tabellen. |
| [GetIsFormulas](./getisformulas/) | Anger om data är formler. |
| [SetIsFormulas](./setisformulas/) | Anger om data är formler. |
| [GetTotalRows](./gettotalrows/) | Hämtar eller anger totalt antal rader att importera från datakällan. -1 betyder alla rader i den angivna datakällan. |
| [SetTotalRows](./settotalrows/) | Hämtar eller anger totalt antal rader att importera från datakällan. -1 betyder alla rader i den angivna datakällan. |
| [GetTotalColumns](./gettotalcolumns/) | Hämtar eller anger totalt antal kolumner att importera från datakällan. -1 betyder alla kolumner i den angivna datakällan. |
| [SetTotalColumns](./settotalcolumns/) | Hämtar eller anger totalt antal kolumner att importera från datakällan. -1 betyder alla kolumner i den angivna datakällan. |
| [GetColumnIndexes](./getcolumnindexes/) | Hämtar eller anger kolumnerna (0-baserade) att importera från datakällan. null betyder att alla kolumner ska importeras. |
| [SetColumnIndexes](./setcolumnindexes/) | Hämtar eller anger kolumnerna (0-baserade) att importera från datakällan. null betyder att alla kolumner ska importeras. |
| [GetDefaultValues](./getdefaultvalues/) | Standardvärdet för värdet i tabellen är null. |
| [SetDefaultValues](./setdefaultvalues/) | Standardvärdet för värdet i tabellen är null. |
| [IsHtmlString](./ishtmlstring/) | Anger om värdet innehåller HTML-taggar. |
| [SetIsHtmlString](./setishtmlstring/) | Anger om värdet innehåller HTML-taggar. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Anger om sammanslagna celler ska kontrolleras. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Anger om sammanslagna celler ska kontrolleras. |
