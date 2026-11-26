---
title: "Title.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Title. Obtiene o establece el texto de la etiqueta de unidad de visualización"
type: docs
url: /es/net/aspose.cells.charts/title/text/
---
## Title.Text property

Obtiene o establece el texto de la etiqueta de unidad de visualización.

```csharp
public override string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);
            
            // Agregue un gráfico y establezca el texto del título del eje de valores
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.ValueAxis.Title.Text = "Sales Amount";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


