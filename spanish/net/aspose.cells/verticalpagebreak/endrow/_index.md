---
title: "VerticalPageBreak.EndRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VerticalPageBreak. Obtiene el índice de fila final del salto de página vertical"
type: docs
url: /es/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Obtiene el índice de fila final del salto de página vertical.

```csharp
public int EndRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un salto de página vertical que abarque las filas 3 a 8 en la columna C (índice 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Obtener el primer salto de página vertical
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Mostrar la fila final del salto de página
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Dado que EndRow es de solo lectura, demostraremos cómo obtenerlo pero no establecerlo
            // La siguiente línea se elimina porque causa un error de compilación:
            // vpb.EndRow = 10;
            
            // En su lugar, agregaremos otro salto de página con una fila final diferente
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Ver también

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


