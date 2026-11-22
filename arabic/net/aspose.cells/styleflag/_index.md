---
title: "الفئة StyleFlag"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.StyleFlag. تمثل العلامات التي تشير إلى خصائص التنسيق المطبقة."
type: docs
url: /ar/net/aspose.cells/styleflag/
---
## StyleFlag class

يمثل العلامات التي تشير إلى خصائص التنسيق المطبقة.

```csharp
public class StyleFlag
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [StyleFlag](styleflag/)() | ينشئ كائنًا بجميع العلامات مضبوطة على false. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | سيتم تطبيق إعداد المحاذاة. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | سيتم تطبيق جميع الخصائص. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | سيتم تطبيق جميع إعدادات الحدود. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | سيتم تطبيق إعدادات الحد السفلي. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | سيتم تطبيق إعداد تظليل الخلية. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | سيتم تطبيق إعدادات الحدود القطرية السفلية. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | سيتم تطبيق إعدادات الحدود القطرية العلوية. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | سيتم تطبيق إعدادات الخط. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | سيتم تطبيق إعداد الخط العريض. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | سيتم تطبيق إعداد لون الخط. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | سيتم تطبيق إعداد الخط المائل. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | سيتم تطبيق إعداد اسم الخط. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | سيتم تطبيق إعداد نمط الخط. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | سيتم تطبيق إعداد حجم الخط. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | سيتم تطبيق إعداد شطب الخط. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | سيتم تطبيق إعداد تسطير الخط. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | سيتم تطبيق إعداد إخفاء الصيغة. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | سيتم تطبيق إعداد المحاذاة الأفقية. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | سيتم تطبيق إعداد مستوى المسافة البادئة. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | سيتم تطبيق إعدادات الحد الأيسر. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | سيتم تطبيق إعداد القفل. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | سيتم تطبيق إعداد تنسيق الأرقام. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | سيتم تطبيق إعداد إخفاء الصيغة. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | سيتم تطبيق إعدادات الحد الأيمن. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | سيتم تطبيق إعداد الدوران. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | سيتم تطبيق إعداد التصغير لتناسب. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | سيتم تطبيق إعداد اتجاه النص. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | سيتم تطبيق إعدادات الحد العلوي. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | سيتم تطبيق إعداد المحاذاة العمودية. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | سيتم تطبيق إعداد التفاف النص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // إنشاء كائن نمط جديد
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // إنشاء كائن StyleFlag جديد
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // تطبيق النمط على نطاق من الخلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // احفظ المصنف
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


