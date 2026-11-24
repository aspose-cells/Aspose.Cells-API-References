---
title: "Klasse CalculationCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CalculationCell‑Klasse. Stellt die berechnungsrelevanten Daten einer Zelle dar, die gerade berechnet wird."
type: docs
url: /de/net/aspose.cells/calculationcell/
---
## CalculationCell class

Stellt die für die Berechnung relevanten Daten einer Zelle dar, die gerade berechnet wird.

```csharp
public class CalculationCell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Liefert das Cell-Objekt, das berechnet wird. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Liefert den Spaltenindex der Zelle. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Liefert den Zeilenindex der Zelle. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Liefert das Workbook-Objekt. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Liefert das Worksheet-Objekt, in dem sich die Zelle befindet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Setzt den berechneten Wert für die Zelle. |

### Hinweise

Der Benutzer sollte während des Formelberechnungsprozesses keine Daten im Workbook ändern, da sonst unerwartete Ergebnisse oder Ausnahmen auftreten können. Daher dienen alle von dieser Klasse bereitgestellten Objekte (wie das Cell-Objekt von [`Cell`](./cell/)) ausschließlich dem "Lese"-Zweck.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
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

                // Grundlegende Eigenschaften anzeigen
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Speichere die Arbeitsmappe
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


