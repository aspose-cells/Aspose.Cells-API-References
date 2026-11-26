---
title: "Row.IsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Indica si la fila contiene datos"
type: docs
url: /es/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Indica si la fila contiene datos.

```csharp
public bool IsBlank { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la primera fila (inicialmente vacía)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // Agregar datos a la primera fila
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Crear otra fila vacía
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Comparar el estado de vacío de la fila
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


