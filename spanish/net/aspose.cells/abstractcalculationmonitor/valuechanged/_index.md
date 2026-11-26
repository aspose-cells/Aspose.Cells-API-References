---
title: "AbstractCalculationMonitor.ValueChanged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractCalculationMonitor. Indica si el valor de la celda ha sido cambiado después del cálculo. Debe usarse solo en AfterCalculate"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Indica si el valor de la celda ha sido cambiado después del cálculo. Debe usarse solo en [`AfterCalculate`](../aftercalculate/).

```csharp
public bool ValueChanged { get; }
```

### Ejemplos

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

            // Establecer valor inicial
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";

            // Crear y establecer monitor de cálculo
            CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Primer cálculo
            workbook.CalculateFormula(options);
            Console.WriteLine($"First calculation - Changed: {monitor.Changed}");

            // Cambiar el valor y recalcular
            worksheet.Cells["A1"].Value = 20;
            monitor.Changed = false;
            workbook.CalculateFormula(options);
            Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
        }
    }
}
```

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


