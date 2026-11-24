---
title: "Klasse AbstractCalculationMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AbstractCalculationMonitor Klasse. Überwacht für den Benutzer den Fortschritt der Formelberechnung."
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Überwacht für den Benutzer den Fortschritt der Formelberechnung.

```csharp
public abstract class AbstractCalculationMonitor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Liest den neu berechneten Wert der Zelle. Sollte nur in [`AfterCalculate`](./aftercalculate/) verwendet werden. |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Liest den alten Wert der berechneten Zelle. Sollte nur in [`BeforeCalculate`](./beforecalculate/) und [`AfterCalculate`](./aftercalculate/) verwendet werden. |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Gibt an, ob der Zellenwert nach der Berechnung geändert wurde. Sollte nur in [`AfterCalculate`](./aftercalculate/) verwendet werden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implementieren Sie diese Methode, um nach der Berechnung einer Zelle geschäftliche Logik auszuführen. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implementieren Sie diese Methode, um vor der Berechnung einer Zelle geschäftliche Logik auszuführen. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implementieren Sie diese Methode, um Geschäftslogik auszuführen, wenn Formeln mit zirkulären Verweisen berechnet werden. |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Benutzerdefinierte Implementierung von AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Erstellen Sie eine Instanz von CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Setzen Sie Berechnungsoptionen
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Berechnen Sie Formeln mit dem benutzerdefinierten Monitor
            workbook.CalculateFormula(options);

            // Speichere die Arbeitsmappe
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


