---
title: "VerticalPageBreak.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VerticalPageBreak. Obtiene el índice de fila inicial del salto de página vertical"
type: docs
url: /es/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Obtiene el índice de fila inicial del salto de página vertical.

```csharp
public int StartRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar saltos de página verticales con la fila inicial deseada (2) inicialmente
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Mostrar la propiedad StartRow
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Dado que StartRow es de solo lectura, necesitamos eliminar y volver a agregar para cambiarlo
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Guarda el libro de trabajo
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Ver también

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


