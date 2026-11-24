---
title: "StyleFlag.All"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Alle Eigenschaften werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Alle Eigenschaften werden angewendet.

```csharp
public bool All { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstellen Sie einen Stil mit solidem rotem Hintergrund
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Erstellen Sie ein Style-Flag mit der All-Eigenschaft auf true gesetzt
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Wenden Sie den Stil auf die erste Spalte an
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Überprüfen Sie, ob der Stil auf die Zellen in der Spalte angewendet wurde
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


