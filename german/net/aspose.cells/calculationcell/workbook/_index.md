---
title: "CalculationCell.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationCell-Eigenschaft. Gibt das Workbook-Objekt zurück"
type: docs
url: /de/net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Liefert das Workbook-Objekt.

```csharp
public Workbook Workbook { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorkbookDemo
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

                // Zeigen Sie den Wert der Workbook-Eigenschaft an
                Console.WriteLine("Workbook Name: " + calcCell.Workbook.FileName);
                Console.WriteLine("Workbook Has Macro: " + calcCell.Workbook.HasMacro);
                Console.WriteLine("Workbook Worksheet Count: " + calcCell.Workbook.Worksheets.Count);

                // Demonstrieren Sie verwandte Eigenschaften im Kontext
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Speichere die Arbeitsmappe
                workbook.Save("WorkbookDemo.xlsx");
                Console.WriteLine("Workbook property demonstration completed successfully.");
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

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


