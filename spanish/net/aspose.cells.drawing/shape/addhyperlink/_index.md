---
title: "Shape.AddHyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Añade un hipervínculo a la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Agrega un hipervínculo a la forma.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

Devuelve el nuevo objeto de hipervínculo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Agregar un hipervínculo a la forma usando una cadena URL
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Guarda el libro de trabajo
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


