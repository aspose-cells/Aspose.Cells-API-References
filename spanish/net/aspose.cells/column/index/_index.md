---
title: "Column.Index"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Obtiene el índice de esta columna"
type: docs
url: /es/net/aspose.cells/column/index/
---
## Column.Index property

Obtiene el índice de esta columna.

```csharp
public int Index { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las columnas
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Obtener la colección de columnas
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Demostrar la propiedad Index
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Acceder a la columna por índice
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // Modificar el ancho de la columna usando el índice
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


