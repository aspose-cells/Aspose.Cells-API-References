---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DefaultStyleSettings-Eigenschaft. Gibt/Setzt den Standardwert für die horizontale Ausrichtung"
type: docs
url: /de/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Liest/Setzt den Standardwert für die horizontale Ausrichtung

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Beispiele

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

            // Horizontale Ausrichtung setzen, um die Eigenschaft zu demonstrieren
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


