---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una AutoShape al gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Agrega una AutoShape al gráfico.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | AutoShapeType | Tipo de AutoShape. |
| superior | Int32 | Representa el desplazamiento vertical del cuadro de texto desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | Int32 | Representa el desplazamiento vertical del cuadro de texto desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | Int32 | Representa la altura del cuadro de texto, en unidades de 1/4000 del área del gráfico. |
| ancho | Int32 | Representa el ancho del cuadro de texto, en unidades de 1/4000 del área del gráfico. |

### Valor de retorno

Devuelve un objeto de forma.

### Observaciones

El tipo no pudo ser Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Llame al método AddAutoShapeInChart para añadir una forma de estrella al gráfico
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Establecer propiedades de la forma
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


