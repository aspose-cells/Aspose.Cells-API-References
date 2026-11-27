---
title: "Klass ImageSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ImageSaveOptions-klass. Representerar bildsparalternativ. För avancerad användning, vänligen använd WorkbookRender eller SheetRender"
type: docs
url: /sv/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Representerar bildsparalternativ. För avancerad användning, vänligen använd [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) eller [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Skapar alternativen för att spara bildfil. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Skapar alternativen för att spara bildfil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Ytterligare alternativ för bildskapande. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Hämtar eller anger IStreamProvider för export av objekt. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // Ange destinationssökvägen
            string destPath = "output.png";

            // Skapa bildsparalternativ
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Anpassa sparalternativ
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // Spara arbetsbok med bildalternativ
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


