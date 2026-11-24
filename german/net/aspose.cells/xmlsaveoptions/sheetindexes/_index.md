---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlSaveOptions-Eigenschaft. Stellt die Indizes der exportierten Blätter dar"
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Stellt die Indizes der exportierten Arbeitsblätter dar.

```csharp
public int[] SheetIndexes { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit mehreren Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Fülle einige Daten in allen Blättern ein
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Erstelle eine XmlSaveOptions-Instanz
            XmlSaveOptions options = new XmlSaveOptions();

            // Exportiere zunächst alle Blätter (SheetIndexes ist null)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Setze, um nur das erste und dritte Blatt zu exportieren (Indizes 0 und 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Speichern nur mit ausgewählten Blättern
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Ändere, um nur das zweite Blatt zu exportieren (Index 1)
            options.SheetIndexes = new int[] { 1 };

            // Speichern mit anderer Blattauswahl
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Setze SheetIndexes auf null, um alle Blätter zu exportieren
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Siehe auch

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


