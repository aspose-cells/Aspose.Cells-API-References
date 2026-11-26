---
title: "ListObject.StartColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene la columna inicial del rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

Obtiene la columna inicial del rango.

```csharp
public int StartColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo para la tabla
            worksheet.Cells["E5"].PutValue("ID");
            worksheet.Cells["F5"].PutValue("Name");
            worksheet.Cells["G5"].PutValue("Age");
            
            worksheet.Cells["E6"].PutValue(1);
            worksheet.Cells["F6"].PutValue("John");
            worksheet.Cells["G6"].PutValue(30);
            
            worksheet.Cells["E7"].PutValue(2);
            worksheet.Cells["F7"].PutValue("Alice");
            worksheet.Cells["G7"].PutValue(25);

            // Crear un objeto lista (tabla)
            int startRow = 5;
            int startCol = 4; // Column E (0-based index 4)
            int endRow = 7;
            int endCol = 6; // Column G (0-based index 6)
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(startRow, startCol, endRow, endCol, true)];
            
            // Demostrar la propiedad StartColumn
            Console.WriteLine("Table starts at column index: " + table.StartColumn);
            Console.WriteLine("Table starts at column letter: " + CellsHelper.ColumnIndexToName(table.StartColumn));
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectStartColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


