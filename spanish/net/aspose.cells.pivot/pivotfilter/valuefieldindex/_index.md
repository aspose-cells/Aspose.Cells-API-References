---
title: "PivotFilter.ValueFieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el índice del campo de valor en la región de valores"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

Obtiene el índice del campo de valor en la región de valores.

```csharp
public int ValueFieldIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValueFieldIndexDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
            
            // Agregar filtro de recuento al campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Obtener el filtro y demostrar ValueFieldIndex
            PivotFilter filter = rowField.GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


