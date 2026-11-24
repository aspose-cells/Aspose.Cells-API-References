---
title: "Range.ClearComments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Löscht die Kommentare dieses Bereichs"
type: docs
url: /de/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Löscht die Kommentare dieses Bereichs.

```csharp
public void ClearComments()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Daten und Kommentare zu Zellen hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Erstelle einen Bereich, der Zellen mit Kommentaren enthält
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Lösche Kommentare aus dem Bereich
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Speichere die Arbeitsmappe
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


