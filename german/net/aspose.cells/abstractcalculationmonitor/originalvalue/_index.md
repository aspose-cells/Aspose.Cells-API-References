---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationMonitor-Eigenschaft. Gibt den alten Wert der berechneten Zelle zurück. Sollte nur in BeforeCalculate und AfterCalculate verwendet werden."
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Gibt den alten Wert der berechneten Zelle zurück. Sollte nur in [`BeforeCalculate`](../beforecalculate/) und [`AfterCalculate`](../aftercalculate/) verwendet werden.

```csharp
public object OriginalValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor1 : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyOriginalValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialen Wert festlegen
            worksheet.Cells["A1"].PutValue(10);
            
            // Formel hinzufügen, die den Wert ändert
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Berechnungsmonitor festlegen
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Formeln neu berechnen – dies löst den Monitor aus
            workbook.CalculateFormula(options);
            
            // Den ursprünglichen Wert ändern, um den Monitor zu demonstrieren
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


