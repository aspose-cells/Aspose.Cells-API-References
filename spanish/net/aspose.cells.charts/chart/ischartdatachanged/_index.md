---
title: "Chart.IsChartDataChanged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Detecta si la fuente de datos del gráfico ha cambiado"
type: docs
url: /es/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Detecta si el origen de datos de un gráfico ha cambiado.

```csharp
public bool IsChartDataChanged()
```

### Valor de retorno

Devuelve true si el gráfico ha cambiado, de lo contrario devuelve false

### Observaciones

El método detecta los cambios en la fuente de datos del gráfico antes de renderizar el gráfico al formato de imagen. En la primera llamada a Chart.toImage, los datos de origen del gráfico (p. ej., XValuesParseData, ValuesParseData) se registrarán. Antes de volver a llamar al método Chart.toImage, invoque el método IsChartDataChanged para comprobar si el gráfico necesita volver a renderizarse.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Verificar si los datos del gráfico han cambiado (debería ser false inicialmente)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Modificar los datos del gráfico
                worksheet.Cells["B2"].PutValue(15);

                // Verificar nuevamente si los datos del gráfico han cambiado
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Calcular el gráfico para actualizarlo
                chart.Calculate();

                // Verificar después del cálculo
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


