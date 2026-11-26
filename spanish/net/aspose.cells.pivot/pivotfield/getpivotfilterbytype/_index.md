---
title: "PivotField.GetPivotFilterByType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Obtiene el filtro pivote del campo pivote por tipo."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

Obtiene el filtro de tabla dinámica del campo de tabla dinámica por tipo

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            
            sheet.Cells["B1"].Value = "Count";
            sheet.Cells["B2"].Value = 1;
            sheet.Cells["B3"].Value = 2;
            sheet.Cells["B4"].Value = 3;
            sheet.Cells["B5"].Value = 4;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aplicar filtro de recuento
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Obtener el filtro de recuento
            PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
            
            // Mostrar detalles del filtro
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            Console.WriteLine("Auto Filter: " + filter.AutoFilter);
            
            wb.Save("PivotFilterExample.xlsx");
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


