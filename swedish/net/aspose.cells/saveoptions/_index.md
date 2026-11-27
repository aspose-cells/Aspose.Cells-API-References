---
title: "Klass SaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SaveOptions-klass. Representerar alla sparalternativ"
type: docs
url: /sv/net/aspose.cells/saveoptions/
---
## SaveOptions class

Representerar alla sparalternativ

```csharp
public class SaveOptions
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indikerar om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar formatet för sparad fil. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för SmartArt ska uppdateras. Standardvärdet är falskt. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Skapa sparalternativ – spara som CSV
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            
            // Skapa inläsningsalternativ för CSV
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Spara om arbetsboken med hjälp av alternativen
            Workbook resavedWorkbook = Cells_Type_SaveOptions(workbook, saveOptions, loadOptions);

            // Spara resultatet till fil
            resavedWorkbook.Save("output.csv", SaveFormat.Csv);
        }

        public static Workbook Cells_Type_SaveOptions(Workbook wb, SaveOptions optsSave, LoadOptions optsLoad)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                wb.Save(ms, optsSave);
                ms.Position = 0;
                return new Workbook(ms, optsLoad);
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


