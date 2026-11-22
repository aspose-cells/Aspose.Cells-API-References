---
title: "Workbook.SetThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تعيين لون السمة"
type: docs
url: /ar/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

يضبط لون السمة

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ThemeColorType | نوع لون السمة. |
| اللون | اللون | لون السمة |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // عيّن لون السمة لـ Text1 إلى الأخضر
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // تطبيق لون السمة على النمط الافتراضي
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


