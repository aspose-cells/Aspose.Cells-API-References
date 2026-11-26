---
title: "ListObject.EndRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene la fila final del rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Obtiene la fila final del rango.

```csharp
public int EndRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Crear objeto de lista/tabla
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Mostrar EndRow inicial
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Agregar nueva fila a la tabla
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Mostrar EndRow actualizado
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Guarda el libro de trabajo
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


