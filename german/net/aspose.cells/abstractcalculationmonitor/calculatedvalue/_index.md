---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationMonitor-Eigenschaft. Gibt den neu berechneten Wert der Zelle zurück. Sollte nur in AfterCalculate verwendet werden."
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Gibt den neu berechneten Wert der Zelle zurück. Sollte nur in [`AfterCalculate`](../aftercalculate/) verwendet werden.

```csharp
public object CalculatedValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Berechnungskette einrichten
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Monitor erstellen und anhängen
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Berechnung auslösen, die unseren Monitor aufruft
            workbook.CalculateFormula(options);

            // Einen Wert ändern, um die Benachrichtigung über Wertänderungen auszulösen
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


