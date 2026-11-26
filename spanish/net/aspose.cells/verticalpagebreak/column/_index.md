---
title: "VerticalPageBreak.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VerticalPageBreak. Obtiene el índice de columna del salto de página vertical"
type: docs
url: /es/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Obtiene el índice de columna del salto de página vertical.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar saltos de página verticales en las columnas 4 y 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Obtener la colección de saltos de página verticales
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Mostrar información sobre cada salto de página vertical
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Guarda el libro de trabajo
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


