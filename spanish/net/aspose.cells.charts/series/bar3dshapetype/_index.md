---
title: "Series.Bar3DShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3D"
type: docs
url: /es/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

Obtiene o establece el tipo de forma 3D utilizado con el gráfico de barras o columnas 3D.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de barras 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el tipo de forma de la barra a Cilindro
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Guarda el libro de trabajo
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


