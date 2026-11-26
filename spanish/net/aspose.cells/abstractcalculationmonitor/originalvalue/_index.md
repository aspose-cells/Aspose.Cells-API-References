---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractCalculationMonitor. Obtiene el valor anterior de la celda calculada. Debe usarse solo en BeforeCalculate y AfterCalculate"
type: docs
url: /es/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Obtiene el valor anterior de la celda calculada. Debe usarse solo en [`BeforeCalculate`](../beforecalculate/) y [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Ejemplos

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

            // Establecer valor inicial
            worksheet.Cells["A1"].PutValue(10);
            
            // Agregar fórmula que cambiará el valor
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Establecer monitor de cálculo
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Recalcular fórmulas - esto activará el monitor
            workbook.CalculateFormula(options);
            
            // Cambiar el valor original para demostrar el monitor
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### Ver también

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


