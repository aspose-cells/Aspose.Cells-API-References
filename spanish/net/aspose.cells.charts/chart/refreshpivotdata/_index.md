---
title: "Chart.RefreshPivotData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Actualiza los datos del gráfico desde la tabla dinámica"
type: docs
url: /es/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Actualiza los datos del gráfico desde la tabla dinámica.

```csharp
public void RefreshPivotData()
```

### Observaciones

Recopilaremos datos de la fuente de datos pivote para el informe de la tabla dinámica. Este método solo se usa para recopilar todos los datos en un gráfico dinámico.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a la primera hoja de cálculo
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Crear una tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Añade un gráfico
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Establecer origen de datos del gráfico dinámico
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Actualizar datos dinámicos en el gráfico
            chart.RefreshPivotData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


