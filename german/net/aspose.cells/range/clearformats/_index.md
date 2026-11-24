---
title: "Range.ClearFormats"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Löscht die Formate dieses Bereichs"
type: docs
url: /de/net/aspose.cells/range/clearformats/
---
## Range.ClearFormats method

Löscht die Formate dieses Bereichs.

```csharp
public void ClearFormats()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten mit Formatierung hinzu
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "Formatted Cell";
            cell.GetStyle().Font.IsBold = true;
            cell.GetStyle().ForegroundColor = System.Drawing.Color.Yellow;
            cell.GetStyle().Pattern = BackgroundType.Solid;

            // Erstelle einen Bereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B5");

            try
            {
                // Formate aus dem Bereich löschen
                range.ClearFormats();

                Console.WriteLine("Formats cleared successfully from range A1:B5");
                Console.WriteLine($"Cell A1 value after clearing formats: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell A1 is bold after clearing formats: {worksheet.Cells["A1"].GetStyle().Font.IsBold}");

                // Speichere die Arbeitsmappe
                workbook.Save("ClearFormatsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearFormats: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


