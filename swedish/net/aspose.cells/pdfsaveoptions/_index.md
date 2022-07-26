---
title: PdfSaveOptions
second_title: Aspose.Cells för .NET API-referens
description: Representerar alternativen för att spara pdf-fil.
type: docs
weight: 4500
url: /sv/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Representerar alternativen för att spara pdf-fil.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Skapar alternativen för att spara pdf-fil. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Om AllColumnsInOnePagePerSheet är sant , kommer allt kolumninnehåll på ett ark att matas ut till endast en sida i resultat. Bredden på pappersstorleken för siduppsättningen kommer att ignoreras, och de andra inställningarna för siduppsättningen kommer fortfarande att gälla. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Hämtar och ställer in[`Pdf BookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry) objekt. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Den cachade filmappen används för att lagra en del stora data. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Indikerar om formler ska beräknas innan pdf-filen sparas. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Indikerar om teckensnittskompatibilitet ska kontrolleras för varje tecken i text. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil, kan de visas som block i pdf,image. Ställ in detta på sant för att försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken först. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Gör arbetsboken tom när du har sparat filen. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | Arbetsbok konverteras till pdf kommer enligt PdfCompliance i den här egenskapen. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Om true och katalogen inte finns skapas katalogen automatiskt innan filen sparas. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Hämtar och ställer in tiden för generering av pdf-dokumentet. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Hämtar eller ställer in ett värde som bestämmer vägen[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) exporteras till PDF-fil. Standardvärdet är None. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Hämtar eller ställer in standardspråk för redigering. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil, kan de visas som block i pdf,image. Ställ in standardteckensnittet som MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap är inte inställt, kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa unicode-tecken. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Indikerar om fönstrets namnlist ska visa dokumentets titel. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True för att bädda in true type-teckensnitt. Påverkar endast ASCII-tecken 32-127. Teckensnitt för teckenkoder större än 127 är alltid inbäddade. Teckensnitt är alltid inbäddade för PDF/A-1a, PDF/A-1b standard. Standard är true. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Inställning för rendering av Emf-metafil. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Indikerar om dokumentstruktur ska exporteras. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Hämtar eller ställer in inbäddad teckensnittskodning i pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Hämtar eller ställer in rutnätstyp. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Indikerar om du behöver dölja felet under renderingen. Felet kan vara fel i form, bild, diagramrendering, etc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Indikerar om teckensnittet endast ska bytas ut när cellteckensnittet inte är kompatibelt med det. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Anger om områdena för villkorlig formatering och validering slås samman innan filen sparas. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Om OnePagePerSheet är sant , kommer allt innehåll på ett ark att matas ut till endast en sida som resultat. Pappersstorleken för siduppsättningen kommer att vara ogiltig, och de andra inställningarna för siduppsättningen kommer fortfarande att gälla. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Hämtar och ställer in pdf-optimeringstyp. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Indikerar om en tom sida ska matas ut när det inte finns något att skriva ut. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska sparas. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Hämtar eller ställer in det 0-baserade indexet för den första sidan som ska sparas. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Kontrollera/indikera framsteg för sidsparprocessen. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Ange komprimeringsalgoritmen |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Indikerar vilka sidor som inte kommer att skrivas ut. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Får och sätter producent av genererat pdf-dokument. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indikerar om uppdatering av diagramcachedata |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Hämtar spara filformatet. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Ställ in detta alternativ när säkerhet behövs i xls2pdf-resultat. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indikerar om externt definierade namn sorteras innan filen sparas. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indikerar om du sorterar definierade namn innan filen sparas. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Hämtar eller ställer in visning av texttyp när textbredden är större än cellbredden. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indikerar om uppdatering av smart art-inställning. Standardvärdet är false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Anger om validera sammanslagna celler innan filen sparas. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Får eller ställer in varningsåteruppringning. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Ställer in önskad PPI (pixlar per tum) för omsamplingsbilder och jpeg-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att samplas om. |

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
