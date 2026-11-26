---
title: "Style.HorizontalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el tipo de alineación horizontal del texto en una celda"
type: docs
url: /es/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Obtiene o establece el tipo de alineación horizontal del texto en una celda.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer texto en celdas
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Obtener objetos de estilo
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Establecer alineación horizontal
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Aplicar estilos a las celdas
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Guarda el libro de trabajo
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


