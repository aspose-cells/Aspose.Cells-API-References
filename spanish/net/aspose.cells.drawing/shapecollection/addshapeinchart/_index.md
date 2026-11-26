---
title: "ShapeCollection.AddShapeInChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Agrega una forma al gráfico .Todas las unidades son 1/4000 del área del gráfico.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | El tipo de dibujo. |
| ubicación | PlacementType | el tipo de ubicación. |
| izquierda | Int32 | En unidades de 1/4000 del ancho del área del gráfico. |
| superior | Int32 | En unidades de 1/4000 de la altura del área del gráfico. |
| derecha | Int32 | En unidades de 1/4000 del ancho del área del gráfico. |
| inferior | Int32 | En unidades de 1/4000 de la altura del área del gráfico. |
| imageData | Byte[] | Si la forma no es una imagen o un objeto ole, imageData debe ser nulo. |

### Ver también

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Agrega una forma al gráfico .Todas las unidades son 1/4000 del área del gráfico.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | El tipo de dibujo. |
| ubicación | PlacementType | el tipo de ubicación. |
| izquierda | Int32 | En unidades de 1/4000 del ancho del área del gráfico. |
| superior | Int32 | En unidades de 1/4000 de la altura del área del gráfico. |
| derecha | Int32 | En unidades de 1/4000 del ancho del área del gráfico. |
| inferior | Int32 | En unidades de 1/4000 de la altura del área del gráfico. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Agregar forma al gráfico
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Establecer texto de la forma
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Guardar el libro de trabajo
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


