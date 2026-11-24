---
title: "StyleFlag.HorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung für horizontale Ausrichtung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Die Einstellung für die horizontale Ausrichtung wird angewendet.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten in Zellen erstellen
            worksheet.Cells["A1"].PutValue("Left Aligned");
            worksheet.Cells["B1"].PutValue("Center Aligned");
            worksheet.Cells["C1"].PutValue("Right Aligned");
            
            // Erstelle Stile mit unterschiedlichen horizontalen Ausrichtungen
            Style styleLeft = workbook.CreateStyle();
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            
            Style styleCenter = workbook.CreateStyle();
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            
            Style styleRight = workbook.CreateStyle();
            styleRight.HorizontalAlignment = TextAlignmentType.Right;
            
            // Erstelle Stil-Flags, um nur die horizontale Ausrichtung anzuwenden
            StyleFlag flag = new StyleFlag();
            flag.HorizontalAlignment = true;
            
            // Wende Stile auf Bereiche an
            Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
            rangeLeft.ApplyStyle(styleLeft, flag);
            
            Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
            rangeCenter.ApplyStyle(styleCenter, flag);
            
            Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
            rangeRight.ApplyStyle(styleRight, flag);
            
            // Speichere die Arbeitsmappe
            workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


