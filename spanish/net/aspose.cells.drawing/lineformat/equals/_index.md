---
title: "LineFormat.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LineFormat. Determina si esta instancia tiene el mismo valor que otro objeto LineFormat especificado"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Determina si esta instancia tiene el mismo valor que otro objeto [`LineFormat`](../) especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Object | El objeto [`LineFormat`](../) para comparar con esta instancia. |

### Valor de retorno

true si el valor del parámetro obj es el mismo que el valor de esta instancia; de lo contrario, false. Si obj es null, este método devuelve false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma de línea a la hoja de cálculo
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Obtén el formato de línea de la primera forma
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Compara los formatos de línea usando el método Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Ver también

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


