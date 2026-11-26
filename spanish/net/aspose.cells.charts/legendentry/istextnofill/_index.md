---
title: "LegendEntry.IsTextNoFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Obtiene o establece la ausencia de relleno del texto"
type: docs
url: /es/net/aspose.cells.charts/legendentry/istextnofill/
---
## LegendEntry.IsTextNoFill property

Obtiene o establece sin relleno el texto.

```csharp
public bool IsTextNoFill { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsTextNoFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Acceder a la entrada de leyenda y establecer IsTextNoFill
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.IsTextNoFill = true; // Text will have no fill
            
            // Guarda el libro de trabajo
            workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


