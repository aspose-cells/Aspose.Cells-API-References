---
title: "CalculationCell.CellColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationCell-Eigenschaft. Gibt den Spaltenindex der Zelle zurück"
type: docs
url: /de/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Liefert den Spaltenindex der Zelle.

```csharp
public int CellColumn { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten und eine einfache Formel ein
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Erhalten Sie eine CalculationCell-Instanz über Reflection (ihr Konstruktor ist nicht öffentlich)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Lesen und zeigen Sie den Wert der CellColumn-Eigenschaft an
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Zusätzliche Demonstration verwandter Eigenschaften (optional)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Speichern Sie die Arbeitsmappe (die Datei wird die von uns hinzugefügten Daten enthalten)
                workbook.Save("CellColumnDemo.xlsx");
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


