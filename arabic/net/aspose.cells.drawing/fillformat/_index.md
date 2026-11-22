---
title: "الفئة FillFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.FillFormat class. تُغلف الكائن الذي يمثل تنسيق التعبئة لشكل."
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

يغلف الكائن الذي يمثل تنسيق التعبئة لشكل.

```csharp
public class FillFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | يحصل على نوع التعبئة ويضبطه |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | يرجع اللون المتدرج 1 للتعبئة المحددة. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | يرجع اللون المتدرج 2 للتعبئة المحددة. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | يرجع نوع لون التدرج للتعبئة المحددة. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | يعيد درجة التدرج للملء المحدد. ينطبق فقط على Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | يحصل على كائن [`GradientFill`](./gradientfill/). |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | يعيد نمط التدرج للملء المحدد. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | يعيد نوع التدرج للملء المحدد. ينطبق فقط على Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | يحصل على بيانات صورة الرسم ويضبطها. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | يمثل نمط عرض المنطقة. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | يحصل على كائن [`PatternFill`](./patternfill/). |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | يحصل ويضبط نوع تنسيق الصورة. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | يعيد لون التدرج المسبق للملء المحدد. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | يحصل على ويضبط مقياس تنسيق الصورة. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**مهمل.**) يحصل على نوع مجموعة تنسيق الملء. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | يحصل على كائن [`SolidFill`](./solidfill/). |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | يمثل نوع النسيج للملء المحدد. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | يحصل على كائن [`TextureFill`](./texturefill/). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**مهمل.**) يحصل على نوع الملء ويضبطه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | يحصل على رمز التجزئة. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلون واحد. ينطبق فقط على Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلون مسبق. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | يضبط الملء المحدد إلى تدرج بلونين. ينطبق فقط على Excel 2007. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // إضافة مخطط عمودي إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة بيانات إلى المخطط.
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // تطبيق تعبئة التدرج على منطقة السلسلة
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // احفظ المصنف
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


