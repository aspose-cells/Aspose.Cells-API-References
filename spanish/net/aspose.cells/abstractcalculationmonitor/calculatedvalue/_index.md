---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractCalculationMonitor. Obtiene el valor recién calculado de la celda. Debe usarse solo en AfterCalculate"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Obtiene el valor recién calculado de la celda. Debe usarse solo en [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Ejemplos

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

            // Configurar cadena de cálculo
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Crear y adjuntar monitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Activar cálculo que invocará nuestro monitor
            workbook.CalculateFormula(options);

            // Cambiar un valor para activar la notificación de cambio de valor
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


