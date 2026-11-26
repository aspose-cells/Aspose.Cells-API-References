---
title: "Clase VerticalPageBreak"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.VerticalPageBreak. Encapsula el objeto que representa un salto de página vertical"
type: docs
url: /es/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Encapsula el objeto que representa un salto de página vertical.

```csharp
public class VerticalPageBreak
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Obtiene el índice de columna del salto de página vertical. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Obtiene el índice de fila final del salto de página vertical. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Obtiene el índice de fila inicial del salto de página vertical. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un salto de página vertical en la columna G (índice 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Guarda el libro de trabajo
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Acceder al salto de página vertical agregado
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Mostrar las propiedades del salto de página vertical
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


