---
title: "PivotField.FilterByDate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Filtra por valores de fecha del campo dinámico de fila o columna"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filtra por valores de fecha del campo dinámico de fila o columna.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | PivotFilterType | El tipo de datos de filtrado. |
| dateTime1 | DateTime | La etiqueta de fecha de la condición de filtro |
| dateTime2 | DateTime | La etiqueta de fecha límite superior de la condición de filtro entre |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con fechas
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fecha al área de columnas
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Aplicar filtro de fecha (fechas de septiembre entre 2020-2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guardar resultados
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


