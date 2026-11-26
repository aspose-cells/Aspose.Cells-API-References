---
title: "Bevel.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Bevel. Obtiene y establece el tipo de bisel preestablecido"
type: docs
url: /es/net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Obtiene y establece el tipo de bisel predefinido.

```csharp
public BevelPresetType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Establecer color de la serie
            series.Area.ForegroundColor = Color.Blue;

            // Configurar formato 3D y propiedades del bisel
            Format3D format3D = series.ShapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            // Demostrar el uso de la propiedad Type
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 5;
            topBevel.Height = 2;

            // Guarda el libro de trabajo
            workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


