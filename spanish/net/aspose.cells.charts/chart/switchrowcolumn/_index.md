---
title: "Chart.SwitchRowColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Cambia fila/columna"
type: docs
url: /es/net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Intercambia fila/columna.

```csharp
public bool SwitchRowColumn()
```

### Valor de retorno

False significa que cambiar fila/columna falla.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSwitchRowColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C4"].PutValue(350);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:C4", true);
            
            // Mostrar valores originales de la serie
            Console.WriteLine("Before SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Cambiar fila/columna
            chart.SwitchRowColumn();
            
            // Mostrar valores de series después de cambiar
            Console.WriteLine("\nAfter SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Guarda el libro de trabajo
            workbook.Save("SwitchRowColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


