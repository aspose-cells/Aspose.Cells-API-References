---
title: "Row.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene la celda"
type: docs
url: /es/net/aspose.cells/row/item/
---
## Row indexer

Obtiene la celda.

```csharp
public Cell this[int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| columna | El índice de columna |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Acceder a la primera fila
            Row row = sheet.Cells.Rows[0];
            
            // Establecer contenido HTML con diferentes estilos de color
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Demostrar el uso de la propiedad Item y mostrar los colores
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


