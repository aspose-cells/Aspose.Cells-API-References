---
title: "StyleFlag.BottomBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellungen für den unteren Rand werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Die Einstellungen für den unteren Rand werden angewendet.

```csharp
public bool BottomBorder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit Einstellungen für den unteren Rand
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Erstelle ein StyleFlag und aktiviere die Modifikation des unteren Randes
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Wende den Stil mit dem Flag auf die Zelle A1 an
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
            cell.SetStyle(style, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


