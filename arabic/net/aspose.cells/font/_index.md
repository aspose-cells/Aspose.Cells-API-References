---
title: "الفئة Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Font. تغلف كائن الخط المستخدم في جدول بيانات"
type: docs
url: /ar/net/aspose.cells/font/
---
## Font class

يغلف كائن الخط المستخدم في جدول بيانات.

```csharp
public class Font
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | يحصل ويضبط اللون باستخدام قيمة ARGB ذات 32 بت. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) يحصل ويضبط نوع الحروف الكبيرة للنص. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | يمثل مجموعة الأحرف. |
| [Color](../../aspose.cells/font/color/) { get; set; } | يحصل أو يضبط لون الخط. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | يحصل على ويضبط الحجم المزدوج للخط. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط عريضًا. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على مقطع النص. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط يحتوي على شطب أحادي. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط منخفضًا. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط مرتفعًا. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | يحصل على أو يضبط اسم الـ `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | يحصل على ويضبط نوع المخطط للخط. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | يحصل على ويضبط إزاحة النص، بوحدة النسبة المئوية |
| [Size](../../aspose.cells/font/size/) { get; set; } | يحصل على أو يضبط حجم الخط. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | يحصل على نوع الشطب للنص. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | يحصل على ويضبط لون السمة. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | يحصل على أو يضبط نوع تسطير الخط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | يتحقق مما إذا كان الخطان متساويين. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | يضبط الاسم والمخطط للخط. |
| override [ToString](../../aspose.cells/font/tostring/)() | إرجاع سلسلة تمثل كائن Cell الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية "A1" من ورقة العمل
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Hello Aspose!");

            // الوصول إلى كائن الخط لنمط الخلية
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // ضبط اسم الخط إلى "Times New Roman"
            font.Name = "Times New Roman";

            // ضبط حجم الخط إلى 14
            font.Size = 14;

            // ضبط لون الخط إلى الأحمر
            font.Color = Color.Red;

            // ضبط خصائص الخط الإضافية
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // حفظ ملف Excel
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


