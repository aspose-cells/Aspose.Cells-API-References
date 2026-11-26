---
title: "SparklineGroup.PresetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el tipo de estilo predefinido del grupo de sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Obtiene y establece el tipo de estilo predefinido del grupo de sparkline.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Observaciones

Si esta propiedad está establecida, estas propiedades: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor serán sobrescritas. Por lo tanto, establezca primero la propiedad y luego las demás.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPresetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);
            worksheet.Cells["E1"].PutValue(9);

            // Crear grupo de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 5;
            ca.EndColumn = 5;
            int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[index];

            // Aplicar estilo predefinido
            group.PresetStyle = SparklinePresetStyleType.Style5;

            workbook.Save("SparklinePresetStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


