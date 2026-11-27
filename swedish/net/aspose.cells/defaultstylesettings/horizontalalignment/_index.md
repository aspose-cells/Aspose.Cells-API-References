---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen DefaultStyleSettings. Hämtar/Anger standardvärdet för horisontell justering"
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Hämtar/Anger standardvärdet för horisontell justering

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Ange horisontell justering för att demonstrera egenskapen
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


