---
title: "StyleFlag.Borders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán todas las configuraciones de borders"
type: docs
url: /es/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Se aplicarán todas las configuraciones de bordes.

```csharp
public bool Borders { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo con configuraciones de border
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Crear una bandera de estilo y habilitar borders
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Aplicar el estilo a la celda A1 solo con borders
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


