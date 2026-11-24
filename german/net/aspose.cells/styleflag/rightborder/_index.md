---
title: "StyleFlag.RightBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Einstellungen für den rechten Rand werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Die Einstellungen für den rechten Rand werden angewendet.

```csharp
public bool RightBorder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit Rahmen
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Erstellen Sie ein Style-Flag und aktivieren Sie den rechten Rand
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


