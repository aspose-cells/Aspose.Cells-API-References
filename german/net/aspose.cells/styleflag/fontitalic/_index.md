---
title: "StyleFlag.FontItalic"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Kursivschrift-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontitalic/
---
## StyleFlag.FontItalic property

Die Einstellung für kursiven Text wird angewendet.

```csharp
public bool FontItalic { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle Beispieldaten
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(1200);
            cells["A3"].PutValue("Monitor");
            cells["B3"].PutValue(250);

            // Erstelle Stile
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.Font.IsItalic = true;
            headerStyle.ForegroundColor = Color.LightGray;
            headerStyle.Pattern = BackgroundType.Solid;

            Style italicStyle = workbook.CreateStyle();
            italicStyle.Font.IsItalic = true;

            // Wende Stile mit StyleFlag an
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

            // Speichere die Arbeitsmappe
            workbook.Save("FontItalicDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


