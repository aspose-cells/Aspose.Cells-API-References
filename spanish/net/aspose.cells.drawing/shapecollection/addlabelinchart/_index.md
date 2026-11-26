---
title: "ShapeCollection.AddLabelInChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una etiqueta al gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Agrega una etiqueta al gráfico.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| superior | Int32 | Representa el desplazamiento vertical de la etiqueta desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | Int32 | Representa el desplazamiento vertical de la etiqueta desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | Int32 | Representa la altura de la etiqueta, en unidades de 1/4000 del área del gráfico. |
| ancho | Int32 | Representa el ancho de la etiqueta, en unidades de 1/4000 del área del gráfico. |

### Valor de retorno

Un nuevo objeto Label.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para crear un gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Llamar al método AddLabelInChart con los parámetros (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Establecer propiedades de la etiqueta
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


