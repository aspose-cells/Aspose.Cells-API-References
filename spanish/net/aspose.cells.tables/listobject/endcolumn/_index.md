---
title: "ListObject.EndColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene la columna final del rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Obtiene la columna final del rango.

```csharp
public int EndColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Crear un objeto de lista o tabla
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Mostrar columna final original
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Redimensionar la tabla para incluir una columna más
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Mostrar nueva columna final
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


