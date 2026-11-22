---
title: "Workbook.GetThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحصل على لون السمة"
type: docs
url: /ar/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

يحصل على لون السمة.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ThemeColorType | نوع لون السمة. |

### قيمة الإرجاع

لون السمة.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الحصول على لون السمة لـ Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


