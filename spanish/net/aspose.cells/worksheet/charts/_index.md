---
title: "Worksheet.Charts"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet propiedad. Obtiene una colección de Chart"
type: docs
url: /es/net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Obtiene una colección de [`Chart`](../../../aspose.cells.charts/chart/)

```csharp
public ChartCollection Charts { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyChartsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Acceder a la primera serie y establecer el patrón de relleno
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Solid;
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetPropertyChartsDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


