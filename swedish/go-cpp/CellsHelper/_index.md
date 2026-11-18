---
title: "CellsHelper-klass"
linktitle: "CellsHelper"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CellsHelper-klass. Inkapslar objektet som representerar cellshelper i Go."
type: docs
weight: 200
url: /sv/go-cpp/cellshelper/
---

## CellsHelper class

Tillhandahåller hjälpfunktioner.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Hämtar och anger standardtypen för signifikanta siffror vid utskrift av numeriska värden. Standardvärdet är SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Hämtar och anger standardtypen för signifikanta siffror vid utskrift av numeriska värden. Standardvärdet är SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Hämtar DPI för maskinen. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Hämtar DPI för maskinen. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Hämta bredden på text i enheten punkter. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Hämta versionsnumret. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Hämtar cellens rad- och kolumnindex enligt dess namn. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Hämtar cellnamnet enligt dess rad- och kolumnindex. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Hämtar kolumnnamnet enligt kolumnindex. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Hämtar kolumnindex enligt kolumnnamn. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Hämtar radnamnet enligt radindex. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Hämtar radindex enligt radnamn. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Konvertera dubbelvärdet till datum‑tidsvärdet. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Konvertera datum‑tiden till dubbelvärde. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Hämtar eller anger startvägen, som refereras till av vissa externa formelreferenser. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Hämtar eller anger startvägen, som refereras till av vissa externa formelreferenser. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Hämtar eller anger den alternativa startvägen, som refereras till av vissa externa formelreferenser. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Hämtar eller anger den alternativa startvägen, som refereras till av vissa externa formelreferenser. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Hämtar eller anger biblioteksökvägen som refereras till av vissa externa formelreferenser. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Hämtar eller anger biblioteksökvägen som refereras till av vissa externa formelreferenser. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Hämtar alla använda färger i arbetsboken. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Slår samman några stora xls‑filer till en xls‑fil. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Hämtar mappen för temporära filer som kan användas som datacache. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Anger mappen för temporära filer som kan användas som datacache. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn, returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken kommer att ersättas med ' ', sedan returneras det ombyggda strängvärdet. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn, returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken kommer att ersättas med det angivna tecknet, sedan returneras det ombyggda strängvärdet. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Anger om bladnamnet ska omges av enkla citattecken |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Ställ in detta egenskap till True när du kör på en molnplattform, till exempel: Azure, AWSLambda, etc, |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Ställ in detta egenskap till True när du kör på en molnplattform, till exempel: Azure, AWSLambda, etc, |
