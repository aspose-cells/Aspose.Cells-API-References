---
title: "Chart.PivotSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. El origen son los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es un PivotChart"
type: docs
url: /es/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

La fuente son los datos de la tabla dinámica. Si PivotSource no está vacío, el gráfico es PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Observaciones

Si la tabla dinámica "PivotTable1" está en la hoja de cálculo "Sheet1" del archivo "Book1.xls". El pivotSource podría ser "[Book1.xls]Sheet1!PivotTable1" si el gráfico y la tabla dinámica no están en el mismo libro. Si establece esta propiedad, se perderá la configuración anterior del origen de datos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer el origen de pivote para el gráfico
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Actualizar los datos de pivote y el gráfico
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


