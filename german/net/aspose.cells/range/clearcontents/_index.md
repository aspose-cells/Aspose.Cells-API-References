---
title: "Range.ClearContents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Löscht den Inhalt dieses Bereichs"
type: docs
url: /de/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Löscht den Inhalt dieses Bereichs.

```csharp
public void ClearContents()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten hinzu, um das Löschen zu demonstrieren
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Erstelle einen Bereich, der die Zellen A1:B2 abdeckt
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Zeige den Inhalt des Bereichs vor dem Löschen an
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Rufe ClearContents auf, um alle Werte im Bereich zu entfernen
                range.ClearContents();

                // Zeige den Inhalt des Bereichs nach dem Löschen an
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Speichere die Arbeitsmappe
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


