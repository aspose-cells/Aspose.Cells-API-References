---
title: "Chart.IsReferedByChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Devuelve si la celda es referenciada por el gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/isreferedbychart/
---
## Chart.IsReferedByChart method

Devuelve si la celda es referenciada por el gráfico.

```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | El índice de fila |
| columnIndex | Int32 | El índice de columna |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método IsCellReferedByChart(int,int,int). Este método será eliminado 12 meses después, a partir de abril de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsReferedByChartWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Verificar si la celda B2 (fila 1, columna 1) es referenciada por el gráfico
                bool isReferred = chart.IsReferedByChart(1, 1);
                
                Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
                
                // Verificar una celda que no está en el rango de datos del gráfico
                bool isNotReferred = chart.IsReferedByChart(10, 10);
                Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


