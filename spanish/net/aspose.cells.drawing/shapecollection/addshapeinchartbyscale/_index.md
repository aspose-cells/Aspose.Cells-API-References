---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una forma al gráfico. Todas las unidades son escala porcentual del área del gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Agrega una forma al gráfico. Todas las unidades son escala porcentual del área del gráfico.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | El tipo de dibujo. |
| ubicación | PlacementType | el tipo de ubicación. |
| izquierda | Double | La unidad es la escala porcentual del ancho del área del gráfico. |
| superior | Double | La unidad es la escala porcentual de la altura del área del gráfico. |
| derecha | Double | La unidad es la escala porcentual del ancho del área del gráfico. |
| inferior | Double | La unidad es la escala porcentual de la altura del área del gráfico. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Calcular gráfico
            chart.Calculate();

            // Añade una forma rectangular al gráfico usando coordenadas de escala
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Añade una forma ovalada al gráfico usando coordenadas de escala
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Guarda el libro de trabajo
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Agrega una forma al gráfico .Todas las unidades son 1/4000 del área del gráfico.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | El tipo de dibujo. |
| ubicación | PlacementType | el tipo de ubicación. |
| izquierda | Double | La unidad es la escala porcentual del ancho del área del gráfico. |
| superior | Double | La unidad es la escala porcentual de la altura del área del gráfico. |
| derecha | Double | La unidad es la escala porcentual del ancho del área del gráfico. |
| inferior | Double | La unidad es la escala porcentual de la altura del área del gráfico. |
| imageData | Byte[] | Si la forma no es una imagen o un objeto ole, imageData debe ser nulo. |

### Ver también

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


