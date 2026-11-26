---
title: "ChartTextFrame.DirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Obtiene y establece la dirección del texto"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Obtiene y establece la dirección del texto.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // Agregar una hoja de cálculo devuelve su índice, luego obtenemos la hoja de cálculo por índice
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Acceder y configurar el título
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Demostrar la propiedad DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


