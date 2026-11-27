---
title: "Klass OdsSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OdsSaveOptions-klass. Representerar alternativen för att spara ods‑fil"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/
---
## OdsSaveOptions class

Representerar alternativen för att spara ods-fil.

```csharp
public class OdsSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [OdsSaveOptions](odssaveoptions/#constructor)() | Skapar alternativen för att spara ods‑fil. |
| [OdsSaveOptions](odssaveoptions/#constructor_1)(SaveFormat) | Skapar alternativen för att spara ods‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [GeneratorType](../../aspose.cells/odssaveoptions/generatortype/) { get; set; } | Hämtar och anger generatorn för ods‑filen. |
| [IgnorePivotTables](../../aspose.cells/odssaveoptions/ignorepivottables/) { get; set; } | Anger om pivottabeller ska sparas. |
| [IsStrictSchema11](../../aspose.cells/odssaveoptions/isstrictschema11/) { get; set; } | (**Obsolete.**) Anger om ods‑filen ska sparas som ODF‑format version 1.1. Standard är false. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [OdfStrictVersion](../../aspose.cells/odssaveoptions/odfstrictversion/) { get; set; } | Hämtar och anger ODF‑versionen. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsDemo
    {
        public static void OdsSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa en instans av OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Ställa in egenskaper
            saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
            saveOptions.IsStrictSchema11 = true;
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Spara arbetsboken som ODS-fil med de angivna alternativen
            workbook.Save("OdsSaveOptionsExample.ods", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


