---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotDateTimeRangeGroupSettings. Obtiene la información interna del grupo"
type: docs
url: /es/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Obtiene el interno del grupo.

```csharp
public double Interval { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo con datos de ejemplo
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Agregar datos de fecha de muestra
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Agregar una hoja de cálculo de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Agregar tabla dinámica
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Agregue el campo de fecha al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Agrupar por días con intervalo de 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Dado que Interval es de solo lectura, debemos establecerlo durante la agrupación
            // El intervalo se establece realmente en los parámetros del método GroupBy
            // Aquí solo verificamos el valor del intervalo
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Guarda el libro de trabajo
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


