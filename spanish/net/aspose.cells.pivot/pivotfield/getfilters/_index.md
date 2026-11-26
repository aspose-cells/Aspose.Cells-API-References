---
title: "PivotField.GetFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotField. Obtiene todos los filtros pivot aplicados a este campo pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

Obtiene todos los filtros de tabla dinámica aplicados a este campo de tabla dinámica.

```csharp
public PivotFilter[] GetFilters()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFiltersDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["B1"].Value = "Sales";
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
                worksheet.Cells[$"B{i}"].Value = i * 100;
            }

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aplicar filtro de fecha
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = DateTime.Now;
            DateTime endDate = DateTime.Now.AddDays(5);
            dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
            
            // Obtener y mostrar filtros
            PivotFilter[] filters = dateField.GetFilters();
            Console.WriteLine($"Number of filters applied: {filters.Length}");
            if (filters.Length > 0)
            {
                Console.WriteLine($"Filter type: {filters[0].FilterType}");
                Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
                Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldGetFiltersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


