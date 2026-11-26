---
title: "ChartPoint.ShapeX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Obtiene la coordenada x de la esquina superior izquierda en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que ShapeX esté poblado
            chart.Calculate();

            // Obtenga el primer punto de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor de ShapeX (1/4000 del ancho del gráfico)
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Demuestra el uso de ShapeX para posicionar elementos relativos al punto del gráfico
            // Nota: Dado que ShapeX es de solo lectura, no podemos modificarlo directamente,
            // pero podemos usarlo para posicionar otros elementos
            if (point.ShapeX > 0)
            {
                // Agregar un cuadro de texto alineado con la posición X del punto del gráfico
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Guardar el resultado
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


