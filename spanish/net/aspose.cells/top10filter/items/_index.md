---
title: "Top10Filter.Items"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10Filter. Obtiene y establece el valor superior o inferior que se usa como criterio del filtro"
type: docs
url: /es/net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

Obtiene y establece el valor superior o inferior a usar como criterio de filtro.

```csharp
public int Items { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grapes");
            worksheet.Cells["A6"].PutValue("Mango");
            
            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aplicar filtro top 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Obtener el filtro y demostrar la propiedad Items
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            int itemsCount = filter.GetTop10Value().Items;
            
            Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
        }
    }
}
```

### Ver también

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


