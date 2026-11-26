---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático ocurre cuando el texto dentro de una forma se escala para contener todo el texto."
type: docs
url: /es/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito dentro de ella. El ajuste automático es cuando el texto dentro de una forma se escala para contener todo el texto.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos de la serie
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Acceder a las etiquetas de datos
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // Demostrar la propiedad IsResizeShapeToFitText
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Desactivar el redimensionamiento automático de la forma para ajustar el texto
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Establecer un ancho personalizado que sea más pequeño de lo que normalmente requeriría el texto
                point.DataLabels.Width = 50;
            }

            // Guarda el libro de trabajo
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


