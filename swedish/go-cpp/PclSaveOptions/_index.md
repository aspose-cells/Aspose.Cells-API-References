---
title: "PclSaveOptions klass"
linktitle: "PclSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PclSaveOptions klass. Inkapslar objektet som representerar pclsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/pclsaveoptions/
---

## PclSaveOptions class

Representerar alternativen för att spara en Pcl-fil.

```go

type PclSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPclSaveOptions](./newpclsaveoptions/) | Skapar alternativen för att spara pcl-filen. |
| [NewPclSaveOptions_PaginatedSaveOptions](./newpclsaveoptions_paginatedsaveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetEmbedFont](./getembedfont/) | Indikerar om teckensnittet ska bäddas in i den genererade Pcl-filen. |
| [SetEmbedFont](./setembedfont/) | Indikerar om teckensnittet ska bäddas in i den genererade Pcl-filen. |
| [AddPrinterFont](./addprinterfont/) | Lägger till information om teckensnitt som redan har lagts till skrivaren av tillverkaren. |
| [GetDefaultFont](./getdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken. |
| [SetDefaultFont](./setdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Sätt detta till true för att först försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Sätt detta till true för att först försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Anger om teckensnittet för ett tecken endast ska ersättas när cellens teckensnitt inte är kompatibelt med det. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Anger om teckensnittet för ett tecken endast ska ersättas när cellens teckensnitt inte är kompatibelt med det. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i pagesetup ignoreras, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i pagesetup ignoreras, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [GetIgnoreError](./getignoreerror/) | Anger om du vill dölja felet vid rendering. Felet kan vara i form, bild, diagramrendering osv. |
| [SetIgnoreError](./setignoreerror/) | Anger om du vill dölja felet vid rendering. Felet kan vara i form, bild, diagramrendering osv. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [SetPageIndex](./setpageindex/) | Hämtar eller anger det 0-baserade indexet för den första sidan som ska sparas. |
| [GetPageIndex](./getpageindex/) | Hämtar eller anger det 0-baserade indexet för den första sidan som ska sparas. |
| [SetPageCount](./setpagecount/) | Hämtar eller anger antalet sidor som ska sparas. |
| [GetPageCount](./getpagecount/) | Hämtar eller anger antalet sidor som ska sparas. |
| [GetPrintingPageType](./getprintingpagetype/) | Anger vilka sidor som inte kommer att skrivas ut. |
| [SetPrintingPageType](./setprintingpagetype/) | Anger vilka sidor som inte kommer att skrivas ut. |
| [GetGridlineType](./getgridlinetype/) | Hämtar eller anger rutnätslinjetyp. |
| [SetGridlineType](./setgridlinetype/) | Hämtar eller anger rutnätslinjetyp. |
| [GetGridlineColor](./getgridlinecolor/) | Hämtar eller anger rutnätslinjens färg. |
| [SetGridlineColor](./setgridlinecolor/) | Hämtar eller anger rutnätslinjens färg. |
| [GetTextCrossType](./gettextcrosstype/) | Hämtar eller anger visningstexttyp när textbredden är större än cellbredden. |
| [SetTextCrossType](./settextcrosstype/) | Hämtar eller anger visningstexttyp när textbredden är större än cellbredden. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Hämtar eller anger standardspråk för redigering. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Hämtar eller anger standardspråk för redigering. |
| [GetSheetSet](./getsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Inställning för rendering av EMF-metafil. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Inställning för rendering av EMF-metafil. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Hämtar eller anger anpassade inställningar under rendering. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Hämtar eller anger anpassade inställningar under rendering. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Hämtar eller anger de Excel-specifika renderingsbeteendena som ska tillämpas. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Hämtar eller anger de Excel-specifika renderingsbeteendena som ska tillämpas. |
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
