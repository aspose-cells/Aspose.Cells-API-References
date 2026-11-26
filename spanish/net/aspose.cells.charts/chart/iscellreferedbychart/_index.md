---
title: "Chart.IsCellReferedByChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Devuelve si la celda es referenciada por el gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

Devuelve si la celda es referenciada por el gráfico.

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | El índice de hoja -1 significa la hoja de cálculo que contiene el gráfico actual. |
| rowIndex | Int32 | El índice de fila |
| columnIndex | Int32 | El índice de columna |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Verificar si la celda es referenciada por el gráfico
            bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
            Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


