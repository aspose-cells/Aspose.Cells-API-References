---
title: "StyleFlag.TopBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellungen des oberen Rands werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Die Einstellungen für den oberen Rand werden angewendet.

```csharp
public bool TopBorder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Einen Stil mit oberen Rand-Einstellungen erstellen
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Ein StyleFlag erstellen und die Modifikation des oberen Rands aktivieren
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Den Stil auf Zelle A1 anwenden, wobei nur das Flag für den oberen Rand aktiviert ist
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
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


