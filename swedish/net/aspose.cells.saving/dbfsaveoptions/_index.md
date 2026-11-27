---
title: "Klass DbfSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.DbfSaveOptions klass. Representerar alternativen för att spara dbf‑fil"
type: docs
url: /sv/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

Representerar alternativen för att spara dbf-fil

```csharp
public class DbfSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | Alternativen för att spara .dbf‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner i Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns kommer katalogen att skapas automatiskt innan filen sparas. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.(Ärvd från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | Indikerar om export som strängvärde |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste datan för diagrammet ska cachas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar filformatet för sparning.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art uppdateras. Standardvärdet är false.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varnings‑callback.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa en instans av DbfSaveOptions
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // Ställ in egenskapen ExportAsString
            saveOptions.ExportAsString = true;

            // Spara arbetsboken med DBF‑sparalternativ
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### Se även

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


