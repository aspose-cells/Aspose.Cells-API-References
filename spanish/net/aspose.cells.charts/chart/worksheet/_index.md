---
title: "Chart.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene la hoja de cálculo que contiene este gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Obtiene la hoja de cálculo que contiene este gráfico.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWorksheetDemo
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
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Demostrar el uso de la propiedad Worksheet
            Console.WriteLine("Chart's worksheet index: " + chart.Worksheet.Index);
            Console.WriteLine("Chart's worksheet name: " + chart.Worksheet.Name);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyWorksheetDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


