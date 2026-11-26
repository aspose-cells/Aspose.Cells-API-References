---
title: "Font.SchemeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el tipo de esquema de la fuente"
type: docs
url: /es/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Obtiene y establece el tipo de esquema de la fuente.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySchemeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Font font = cell.GetStyle().Font;
            font.SchemeType = FontSchemeType.Minor;
            font.Name = "Calibri";
            font.Size = 12;

            workbook.Save("FontSchemeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


