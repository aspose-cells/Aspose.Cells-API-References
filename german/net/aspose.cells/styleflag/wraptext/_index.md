---
title: "StyleFlag.WrapText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung zum Zeilenumbruch wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Die Einstellung zum Zeilenumbruch wird angewendet.

```csharp
public bool WrapText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit aktiviertem Zeilenumbruch
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Erstelle ein StyleFlag und aktiviere das WrapText-Flag
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Wende den Stil auf Zelle A1 mit den angegebenen Flags an
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Passe die Zeilenhöhe automatisch an, um den umgebrochenen Text zu sehen
            worksheet.AutoFitRow(0);

            // Speichere die Arbeitsmappe
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


