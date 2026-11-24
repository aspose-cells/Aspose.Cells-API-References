---
title: "CalculationCell.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationCell-Eigenschaft. Gibt das Worksheet-Objekt zurück, in dem sich die Zelle befindet"
type: docs
url: /de/net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Liefert das Worksheet-Objekt, in dem sich die Zelle befindet.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Erstelle eine CalculationCell-Instanz mittels Reflexion, da der Konstruktor nicht öffentlich ist.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Zeigen Sie den Wert der Worksheet-Eigenschaft an
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Worksheet Index: " + calcCell.Worksheet.Index);
                Console.WriteLine("Worksheet Type: " + calcCell.Worksheet.Type);

                // Demonstrieren Sie weitere verwandte Eigenschaften
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Speichere die Arbeitsmappe
                workbook.Save("WorksheetDemo.xlsx");
                Console.WriteLine("Worksheet property demonstration completed successfully.");
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


