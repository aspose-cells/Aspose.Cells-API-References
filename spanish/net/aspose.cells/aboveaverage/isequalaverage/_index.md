---
title: "AboveAverage.IsEqualAverage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AboveAverage. Obtenga o establezca la bandera que indica si los criterios aboveAverage y belowAverage son inclusivos del propio promedio o exclusivos de ese valor. true indica incluir el valor promedio en los criterios. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Obtenga o establezca la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en los criterios. El valor predeterminado es false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
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
            fc.Style.BackgroundColor = Color.LightBlue;

            // Demostrar la propiedad IsEqualAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Rellene datos de ejemplo
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


