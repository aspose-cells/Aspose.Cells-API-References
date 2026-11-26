---
title: "ChartPoint.ShapeWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el ancho en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Obtiene el ancho en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Calcule el gráfico para asegurar que las propiedades de forma estén disponibles
            chart.Calculate();
            
            // Obtener el primer punto del gráfico en la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Muestre el valor actual de ShapeWidth (en 1/4000 del ancho del gráfico)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Muestre el ancho en píxeles
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Nota: ShapeWidth es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el ancho, necesitaríamos modificar el tamaño del gráfico u otras propiedades
            
            // Guardar el resultado
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


