---
title: "Clase HorizontalPageBreak"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HorizontalPageBreak. Encapsula el objeto que representa un salto de página horizontal"
type: docs
url: /es/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Encapsula el objeto que representa un salto de página horizontal.

```csharp
public class HorizontalPageBreak
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Obtiene el índice de columna final de este salto de página horizontal. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Obtiene el índice de fila basado en cero. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Obtiene el índice de columna inicial de este salto de página horizontal. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade un salto de página en la celda Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Obtén el salto de página horizontal recién añadido
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Muestra las propiedades del salto de página horizontal
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Guarda el libro de trabajo
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


