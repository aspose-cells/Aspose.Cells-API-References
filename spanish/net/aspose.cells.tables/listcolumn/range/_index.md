---
title: "ListColumn.Range"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumn. Obtiene el rango de esta columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Obtiene el rango de esta columna de lista.

```csharp
public Range Range { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de ejemplo para crear un objeto de lista
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Crear un objeto de lista
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Obtenga la primera columna de lista
            ListColumn listCol = listObj.ListColumns[0];
            
            // Acceda al rango de la columna de lista
            Aspose.Cells.Range range = listCol.Range;
            
            // Muestre la información del rango
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Modifique celdas en el rango
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


