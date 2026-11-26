---
title: "Title.X"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Title. Obtiene o establece la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/title/x/
---
## Title.X property

Obtiene o establece la coordenada X de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad Title.XRatioToChart, en su lugar. X = XRatioToChart * 4000; Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Agregue un gráfico y establezca los datos
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Establezca las propiedades del título del gráfico con la posición X
            chart.Title.Text = "Sample Chart";
            chart.Title.X = 200; // Demonstrating X property usage
            chart.Title.Y = 50;

            // Guarda el libro de trabajo
            workbook.Save("TitlePropertyXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


