---
title: "Enumeración SparklineAxisMinMaxType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.SparklineAxisMinMaxType enum. Representa los tipos de valor mínimo y máximo para el eje vertical de la sparkline."
type: docs
url: /es/net/aspose.cells.charts/sparklineaxisminmaxtype/
---
## SparklineAxisMinMaxType enumeration

Representa los tipos de valor mínimo y máximo para el eje vertical de la sparkline.

```csharp
public enum SparklineAxisMinMaxType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| AutoIndividual | `0` | Automático para cada sparkline. |
| Group | `1` | Mismo para todas las sparklines del grupo. |
| Custom | `2` | Valor personalizado para la sparkline. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineAxisMinMaxTypeDemo
    {
        public static void SparklineAxisMinMaxTypeExample()
        {
            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Define el CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Añade un grupo de sparkline a la hoja de cálculo
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Establece propiedades para el grupo de sparkline
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Crea CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Establecer propiedades adicionales
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


