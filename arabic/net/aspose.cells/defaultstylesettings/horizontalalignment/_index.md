---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DefaultStyleSettings. تحصل/تضبط القيمة الافتراضية للمحاذاة الأفقية"
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

الحصول/تعيين القيمة الافتراضية للمحاذاة الأفقية

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### أمثلة

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

            // تعيين المحاذاة الأفقية لتوضيح الخاصية
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


