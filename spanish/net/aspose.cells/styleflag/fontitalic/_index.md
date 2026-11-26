---
title: "StyleFlag.FontItalic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración Font italic"
type: docs
url: /es/net/aspose.cells/styleflag/fontitalic/
---
## StyleFlag.FontItalic property

Se aplicará la configuración de cursiva de fuente.

```csharp
public bool FontItalic { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de ejemplo
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(1200);
            cells["A3"].PutValue("Monitor");
            cells["B3"].PutValue(250);

            // Crear estilos
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.Font.IsItalic = true;
            headerStyle.ForegroundColor = Color.LightGray;
            headerStyle.Pattern = BackgroundType.Solid;

            Style italicStyle = workbook.CreateStyle();
            italicStyle.Font.IsItalic = true;

            // Aplicar estilos con StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontBold = true;
            headerFlag.FontItalic = true;
            headerFlag.CellShading = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            Aspose.Cells.Range dataRange = cells.CreateRange(1, 0, 2, 1);
            StyleFlag italicFlag = new StyleFlag();
            italicFlag.FontItalic = true;
            dataRange.ApplyStyle(italicStyle, italicFlag);

            // Guarda el libro de trabajo
            workbook.Save("FontItalicDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


