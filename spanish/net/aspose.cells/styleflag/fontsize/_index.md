---
title: "StyleFlag.FontSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del tamaño de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/fontsize/
---
## StyleFlag.FontSize property

Se aplicará la configuración de tamaño de fuente.

```csharp
public bool FontSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Sample Text");

            Style style = workbook.CreateStyle();
            style.Font.Size = 18;
            style.Font.IsBold = true;

            StyleFlag styleFlag = new StyleFlag
            {
                FontSize = true,
                FontBold = true
            };

            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A1");
            range.ApplyStyle(style, styleFlag);

            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


