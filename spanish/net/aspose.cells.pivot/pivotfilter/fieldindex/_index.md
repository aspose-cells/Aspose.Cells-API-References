---
title: "PivotFilter.FieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el índice del campo origen al que se aplica este filtro pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Obtiene el índice del campo origen al que se aplica este filtro dinámico.

```csharp
public int FieldIndex { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar filtro
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField pivotField = pivotTable.PageFields[0];
            
            // Crear colección de filtros pivote y agregar filtro
            PivotFilterCollection filters = pivotTable.PivotFilters;
            int filterIndex = filters.Add(0, PivotFilterType.Count);
            PivotFilter filter = filters[filterIndex];
            
            // Demostrar la propiedad FieldIndex
            Console.WriteLine("Field Index: " + filter.FieldIndex);

            // Guarda el libro de trabajo
            workbook.Save("PivotFilterFieldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


