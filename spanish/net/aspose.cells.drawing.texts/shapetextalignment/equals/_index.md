---
title: "ShapeTextAlignment.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeTextAlignment. Determina si esta instancia tiene el mismo valor que otro objeto ShapeTextAlignment especificado"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Determina si esta instancia tiene el mismo valor que otro objeto [`ShapeTextAlignment`](../) especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Object | El objeto [`ShapeTextAlignment`](../) para comparar con esta instancia. |

### Valor de retorno

true si el valor del parámetro obj es el mismo que el valor de esta instancia; de lo contrario, false. Si obj es null, este método devuelve false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma para comparar la alineación de texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Obtener la alineación de texto de otra forma para comparar
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


