---
title: "Worksheet.ListObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene todos los ListObjects en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Obtiene todos los ListObjects en esta hoja de cálculo.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Crear un ListObject (tabla)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Redimensionar la tabla para incluir más filas
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Agregar más datos a la tabla extendida
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Acceder a la tabla a través de la propiedad ListObjects
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


