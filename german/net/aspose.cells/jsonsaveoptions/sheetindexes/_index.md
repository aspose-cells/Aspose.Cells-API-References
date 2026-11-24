---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt die Indizes der exportierten Arbeitsblätter an"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

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

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit mehreren Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Einige Daten in jedem Arbeitsblatt einfügen
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // JsonSaveOptions-Instanz erstellen
            JsonSaveOptions options = new JsonSaveOptions();

            // Aktuelle SheetIndexes anzeigen (standardmäßig null – exportiert alle Arbeitsblätter)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Setze, um nur das erste und dritte Blatt zu exportieren (Indizes 0 und 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // In JSON mit ausgewählten Arbeitsblättern speichern
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Durch Laden des JSON überprüfen
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Ändere, um nur das zweite Blatt zu exportieren (Index 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Export eines einzelnen Arbeitsblatts überprüfen
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


