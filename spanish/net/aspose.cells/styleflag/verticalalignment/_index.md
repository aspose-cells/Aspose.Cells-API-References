---
title: "StyleFlag.VerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de alineación vertical"
type: docs
url: /es/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Se aplicará la configuración de alineación vertical.

```csharp
public bool VerticalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Cree un estilo con alineación vertical
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Cree una bandera de estilo para aplicar solo alineación vertical y color de fuente
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Aplique el estilo a la primera fila con la bandera de estilo
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Establezca algún texto en las celdas para ver el efecto
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Guarda el libro de trabajo
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


