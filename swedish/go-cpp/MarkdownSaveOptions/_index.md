---
title: "MarkdownSaveOptions klass"
linktitle: "MarkdownSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "MarkdownSaveOptions-klass. Inkapslar objektet som representerar markdownsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Representerar sparalternativen för markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Skapar alternativ för att spara markdown-dokument |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetEncoding](./getencoding/) | Hämtar och anger standardkodning. |
| [SetEncoding](./setencoding/) | Hämtar och anger standardkodning. |
| [GetFormatStrategy](./getformatstrategy/) | Hämtar och anger formatstrategi när cellvärdet exporteras som sträng. |
| [SetFormatStrategy](./setformatstrategy/) | Hämtar och anger formatstrategi när cellvärdet exporteras som sträng. |
| [GetLineSeparator](./getlineseparator/) | Hämtar och anger radseparatorn. |
| [SetLineSeparator](./setlineseparator/) | Hämtar och anger radseparatorn. |
| [GetTableHeaderType](./gettableheadertype/) | Hämtar och anger hur rubriken för tabellen sätts. |
| [SetTableHeaderType](./settableheadertype/) | Hämtar och anger hur rubriken för tabellen sätts. |
| [GetSheetSet](./getsheetset/) | Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Hämta ImageOrPrintOptions‑objektet innan export. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Anger om bilder sparas i Base64-format till Markdown. Standardvärdet är true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Anger om bilder sparas i Base64-format till Markdown. Standardvärdet är true. |
| [GetCalculateFormula](./getcalculateformula/) | Anger om formler ska beräknas innan markdown-filen sparas. |
| [SetCalculateFormula](./setcalculateformula/) | Anger om formler ska beräknas innan markdown-filen sparas. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Anger om hyperlänkar ska exporteras med referensdefinitioner istället för inline-format. Standardvärdet är false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Anger om hyperlänkar ska exporteras med referensdefinitioner istället för inline-format. Standardvärdet är false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Anger om kolumnjustering är aktiverad för genererade Markdown-tabeller. När den är aktiverad justeras kolumnerna genom att fylla cellinnehållet med det angivna tecknet (vanligtvis ' ' för mellanslag). Sätt till '\\0' för att inaktivera kolumnjustering (standard). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Anger om kolumnjustering är aktiverad för genererade Markdown-tabeller. När den är aktiverad justeras kolumnerna genom att fylla cellinnehållet med det angivna tecknet (vanligtvis ' ' för mellanslag). Sätt till '\\0' för att inaktivera kolumnjustering (standard). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Anger om tomma rader i kalkylbladet ska behandlas som tabellseparatorer vid export till Markdown. Standardvärdet är false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Anger om tomma rader i kalkylbladet ska behandlas som tabellseparatorer vid export till Markdown. Standardvärdet är false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Anger hur OfficeMath-objekt exporteras till Markdown. Standardvärdet är Image. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Anger hur OfficeMath-objekt exporteras till Markdown. Standardvärdet är Image. |
| [GetSaveFormat](./getsaveformat/) | Hämtar formatet för sparad fil. |
| [GetClearData](./getcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [SetClearData](./setcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [GetMergeAreas](./getmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [SetMergeAreas](./setmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [GetCreateDirectory](./getcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [SetCreateDirectory](./setcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [GetSortNames](./getsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [SetSortNames](./setsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [GetSortExternalNames](./getsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [SetSortExternalNames](./setsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
