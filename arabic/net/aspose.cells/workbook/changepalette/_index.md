---
title: "Workbook.ChangePalette"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تغير لوحة الألوان للجدول في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

يغيّر لوحة الألوان لجدول البيانات في الفهرس المحدد.

```csharp
public void ChangePalette(Color color, int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | بنية اللون. |
| فهرس | Int32 | فهرس لوحة الألوان، 0 - 55. |

### ملاحظات

لوحة الألوان تحتوي على 56 مدخلًا، كل منها ممثل بقيمة RGB.

إذا قمت بتعيين لون غير موجود في لوحة الألوان، فلن يُطبق.

لذا إذا أردت تعيين لون مخصص، يرجى تعديل لوحة الألوان أولاً.

ما يلي هو لوحة الألوان القياسية.

| **Color** | **Red** | **أخضر** | **أزرق** |
| --- | --- | --- | --- |
| أسود | 0 | 0 | 0 |
| أبيض | 255 | 255 | 255 |
| أحمر | 255 | 0 | 0 |
| ليموني | 0 | 255 | 0 |
| أزرق | 0 | 0 | 255 |
| أصفر | 255 | 255 | 0 |
| أرجواني | 255 | 0 | 255 |
| سماوي | 0 | 255 | 255 |
| كستنائي | 128 | 0 | 0 |
| أخضر | 0 | 128 | 0 |
| كحلي | 0 | 0 | 128 |
| زيتوني | 128 | 128 | 0 |
| بنفسجي | 128 | 0 | 128 |
| تركوازي | 0 | 128 | 128 |
| فضي | 192 | 192 | 192 |
| رمادي | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| اللون20 | 204 | 255 | 255 |
| اللون21 | 102 | 0 | 102 |
| اللون22 | 255 | 128 | 128 |
| اللون23 | 0 | 102 | 204 |
| اللون24 | 204 | 204 | 255 |
| اللون25 | 0 | 0 | 128 |
| اللون26 | 255 | 0 | 255 |
| اللون27 | 255 | 255 | 0 |
| اللون28 | 0 | 255 | 255 |
| اللون29 | 128 | 0 | 128 |
| اللون30 | 128 | 0 | 0 |
| اللون31 | 0 | 128 | 128 |
| اللون32 | 0 | 0 | 255 |
| اللون33 | 0 | 204 | 255 |
| اللون34 | 204 | 255 | 255 |
| اللون35 | 204 | 255 | 204 |
| اللون36 | 255 | 255 | 153 |
| اللون37 | 153 | 204 | 255 |
| اللون38 | 255 | 153 | 204 |
| اللون39 | 204 | 153 | 255 |
| اللون40 | 255 | 204 | 153 |
| اللون41 | 51 | 102 | 255 |
| اللون42 | 51 | 204 | 204 |
| اللون43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodChangePaletteWithColorInt32Demo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            
            // تغيير لون لوحة الألوان عند الفهرس 55
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط باستخدام لون لوحة الألوان المعدل
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


