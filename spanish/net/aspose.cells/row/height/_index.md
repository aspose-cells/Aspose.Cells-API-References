---
title: "Row.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene y establece la altura de la fila en unidades de puntos"
type: docs
url: /es/net/aspose.cells/row/height/
---
## Row.Height property

Obtiene y establece la altura de la fila en unidades de puntos.

```csharp
public double Height { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la altura de la fila para la primera fila
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Agregar algunos datos a la fila
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Verificar y mostrar la altura de la fila
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Guarda el libro de trabajo
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


