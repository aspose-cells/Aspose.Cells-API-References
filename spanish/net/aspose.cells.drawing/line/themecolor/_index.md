---
title: "Line.ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Obtiene y establece el color del tema"
type: docs
url: /es/net/aspose.cells.drawing/line/themecolor/
---
## Line.ThemeColor property

Obtiene y establece el color del tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Observaciones

Si el color de primer plano no es un color de tema, se devolverá NULL.

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Series 1");
            sheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 2; i <= 6; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i-1));
                sheet.Cells["B" + i].PutValue(i * 10);
                sheet.Cells["C" + i].PutValue(i * 15);
            }

            // Agregar un gráfico de líneas
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("B1:C6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Personalizar la apariencia de la serie con ThemeColor
            var seriesThemes = new List<ThemeColorType> { 
                ThemeColorType.Accent1, 
                ThemeColorType.Accent2 
            };

            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                chart.NSeries[i].Border.ThemeColor = new ThemeColor(seriesThemes[i], 0.6);
                chart.NSeries[i].Border.Style = LineType.Solid;
                chart.NSeries[i].Border.Weight = WeightType.MediumLine;
            }

            // Guarda el libro de trabajo
            workbook.Save("LineChartWithThemeColor.xlsx");
        }
    }
}
```

### Ver también

* class [ThemeColor](../../../aspose.cells/themecolor/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


