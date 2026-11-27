---
title: "Klass XmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XmlSaveOptions‑klass. Representerar alternativen för att spara arbetsboken som en XML‑fil"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/
---
## XmlSaveOptions class

Representerar alternativen för att spara arbetsboken som en xml-fil.

```csharp
public class XmlSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [XmlSaveOptions](xmlsaveoptions/)() | Skapar alternativ för att spara XML‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [DataAsAttribute](../../aspose.cells/xmlsaveoptions/dataasattribute/) { get; set; } | Anger om data exporteras som attribut för elementet. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/xmlsaveoptions/exportarea/) { get; set; } | Hämtar eller anger exportintervallet. |
| [HasHeaderRow](../../aspose.cells/xmlsaveoptions/hasheaderrow/) { get; set; } | Anger om intervallet innehåller en rubrikrad. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SheetIndexes](../../aspose.cells/xmlsaveoptions/sheetindexes/) { get; set; } | Representerar indexen för exporterade blad. |
| [SheetNameAsElementName](../../aspose.cells/xmlsaveoptions/sheetnameaselementname/) { get; set; } | Anger om bladets namn exporteras som elementets namn. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |
| [XmlMapName](../../aspose.cells/xmlsaveoptions/xmlmapname/) { get; set; } | Anger om XML‑karta exporteras i filen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsDemo
    {
        public static void XmlSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Skapa en instans av XmlSaveOptions
            XmlSaveOptions saveOptions = new XmlSaveOptions();

            // Ställa in egenskaper
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 };
            saveOptions.HasHeaderRow = true;
            saveOptions.SheetIndexes = new int[] { 0 };
            saveOptions.XmlMapName = "MyXmlMap";
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = false;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Spara arbetsboken som en XML‑fil
            workbook.Save("XmlSaveOptionsExample.xml", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


