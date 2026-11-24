---
title: "Font.SchemeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schriftart-Eigenschaft. Gibt den Schema-Typ der Schriftart zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Liest und setzt den Schematyp der Schriftart.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


