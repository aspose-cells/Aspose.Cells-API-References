---
title: "MarkdownLoadOptions Class"
linktitle: "MarkdownLoadOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "MarkdownLoadOptions class. Inkapslar objektet som representerar markdownloadoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/markdownloadoptions/
---

## MarkdownLoadOptions class

Representerar alternativen för att läsa in markdown-dokumentet.

```go

type MarkdownLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewMarkdownLoadOptions](./newmarkdownloadoptions/) | Standardkonstruktor. |
| [NewMarkdownLoadOptions_AbstractTextLoadOptions](./newmarkdownloadoptions_abstracttextloadoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetHasFormula](./gethasformula/) | Indikerar om texten är en formel om den börjar med "=". |
| [SetHasFormula](./sethasformula/) | Indikerar om texten är en formel om den börjar med "=". |
| [GetEncoding](./getencoding/) | Hämtar och anger standardkodningen. Gäller endast för csv-filer. |
| [SetEncoding](./setencoding/) | Hämtar och anger standardkodningen. Gäller endast för csv-filer. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Anger strategin för att tillämpa stil för analyserade värden när en strängvärde konverteras till nummer eller datum/tid. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Anger strategin för att tillämpa stil för analyserade värden när en strängvärde konverteras till nummer eller datum/tid. |
| [GetConvertNumericData](./getconvertnumericdata/) | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true. |
| [SetConvertNumericData](./setconvertnumericdata/) | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true. |
| [GetKeepPrecision](./getkeepprecision/) | Anger om en strängvärde inte ska analyseras om längden är 15. |
| [SetKeepPrecision](./setkeepprecision/) | Anger om en strängvärde inte ska analyseras om längden är 15. |
| [GetLoadFormat](./getloadformat/) | Hämtar inläsningsformatet. |
| [GetPassword](./getpassword/) | Hämtar och anger lösenordet för arbetsboken. |
| [SetPassword](./setpassword/) | Hämtar och anger lösenordet för arbetsboken. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Anger om formeln ska analyseras när filen läses. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Anger om formeln ska analyseras när filen läses. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Anger om pivottabellens cachade poster ska analyseras vid inläsning av filen. Standardvärdet är false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Anger om pivottabellens cachade poster ska analyseras vid inläsning av filen. Standardvärdet är false. |
| [SetPaperSize](./setpapersize/) | Ställer in standardpappersstorlek för utskrift från standardskrivarens inställning. |
| [GetLanguageCode](./getlanguagecode/) | Hämtar eller anger användargränssnittsspråket för arbetsboksversionen baserat på CountryCode som har sparat filen. |
| [SetLanguageCode](./setlanguagecode/) | Hämtar eller anger användargränssnittsspråket för arbetsboksversionen baserat på CountryCode som har sparat filen. |
| [GetRegion](./getregion/) | Hämtar eller anger de regionala inställningarna som används för arbetsboken som ska läsas in. |
| [SetRegion](./setregion/) | Hämtar eller anger de regionala inställningarna som används för arbetsboken som ska läsas in. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken |
| [GetInterruptMonitor](./getinterruptmonitor/) | Hämtar och anger avbrottsmotorn. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Hämtar och anger avbrottsmotorn. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [GetCheckDataValid](./getcheckdatavalid/) | Kontrollera om data är giltiga i mallfilen. |
| [SetCheckDataValid](./setcheckdatavalid/) | Kontrollera om data är giltiga i mallfilen. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K, till exempel via Cell.PutValue(string), får du ett Undantag om detta egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera det kompletta strängvärdet till andra filformat såsom CSV. Däremot, om du har angett ett sådant värde som är ogiltigt för Excel-filformatet, bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K, till exempel via Cell.PutValue(string), får du ett Undantag om detta egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera det kompletta strängvärdet till andra filformat såsom CSV. Däremot, om du har angett ett sådant värde som är ogiltigt för Excel-filformatet, bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Om de oparserade data ska behållas i minnet för arbetsboken när den läses in från mallfilen. Standard är true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Om de oparserade data ska behållas i minnet för arbetsboken när den läses in från mallfilen. Standard är true. |
| [GetLoadFilter](./getloadfilter/) | Filtret som anger hur data ska läsas in. |
| [SetLoadFilter](./setloadfilter/) | Filtret som anger hur data ska läsas in. |
| [GetMemorySetting](./getmemorysetting/) | Hämtar eller anger minnesläget för inläst arbetsbok. |
| [SetMemorySetting](./setmemorysetting/) | Hämtar eller anger minnesläget för inläst arbetsbok. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Hämtar och anger auto‑fitter‑alternativen |
| [SetAutoFitterOptions](./setautofitteroptions/) | Hämtar och anger auto‑fitter‑alternativen |
| [GetAutoFilter](./getautofilter/) | Anger om data ska autofilteras vid inläsning av filerna. |
| [SetAutoFilter](./setautofilter/) | Anger om data ska autofilteras vid inläsning av filerna. |
| [GetFontConfigs](./getfontconfigs/) | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för arbetsboken som använder dessa LoadOptions för inläsning. |
| [SetFontConfigs](./setfontconfigs/) | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för arbetsboken som använder dessa LoadOptions för inläsning. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Anger om onödiga former ska ignoreras. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Anger om onödiga former ska ignoreras. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är false. |
