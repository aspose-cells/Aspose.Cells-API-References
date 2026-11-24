---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationMonitor-Eigenschaft. Gibt an, ob der Zellenwert nach der Berechnung geändert wurde. Sollte nur in AfterCalculate verwendet werden"
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Ob der Wert der Zelle nach der Berechnung geändert wurde. Sollte nur in [`AfterCalculate`](../aftercalculate/) verwendet werden.

```csharp
public bool ValueChanged { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor2 : AbstractCalculationMonitor
    {
        public bool Changed { get; set; }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Changed = true;
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyValueChangedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialen Wert festlegen
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // Berechnungsmonitor erstellen und festlegen
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Erste Berechnung
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // Wert ändern und neu berechnen
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


