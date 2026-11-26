---
title: "AboveAverage.StdDev"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AboveAverage. Obtenga o establezca el número de desviaciones estándar que se incluirán por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3, inclusive 0 y 3. Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0"
type: docs
url: /es/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Obtenga o establezca el número de desviaciones estándar para incluir por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0.

```csharp
public int StdDev { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Rellene datos de ejemplo
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


