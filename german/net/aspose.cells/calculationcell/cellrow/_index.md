---
title: "CalculationCell.CellRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationCell-Eigenschaft. Gibt den Zeilenindex der Zelle zurück"
type: docs
url: /de/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Liefert den Zeilenindex der Zelle.

```csharp
public int CellRow { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
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

                // Zeigen Sie den Wert der CellRow-Eigenschaft an
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // Demonstrieren Sie verwandte Eigenschaften im Kontext
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // Speichere die Arbeitsmappe
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


