---
title: "ChartPoint.RadiusPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el radio del pastel de burbuja o donut en unidades de píxeles después de llamar al método Chart.Calculate."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Obtiene el radio de la burbuja, pastel o rosquilla en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestra el valor actual del radio
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Nota: RadiusPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el radio, necesitamos ajustar el tamaño del gráfico o otras propiedades
            // que afectan el tamaño del punto indirectamente

            // Ejemplo de cómo cambiar el tamaño del gráfico afecta al radio
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Muestra el nuevo valor del radio después de redimensionar el gráfico
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Guardar el resultado
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


