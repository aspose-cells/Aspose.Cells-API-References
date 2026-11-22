---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يدرج كائن WordArt إلى المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

يدرج كائن WordArt إلى المخطط.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تأثير | MsoPresetTextEffect | نوع تأثير النص المسبق mso. |
| نص | String | نص WordArt. |
| fontName | String | اسم الخط. |
| الحجم | Int32 | حجم الخط |
| fontBold | منطقي | يشير إلى ما إذا كان الخط عريضًا. |
| fontItalic | منطقي | يشير إلى ما إذا كان الخط مائلًا. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من الزاوية العليا اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | Int32 | يمثل الإزاحة العمودية للشكل من الزاوية العليا اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | Int32 | يمثل ارتفاع الشكل بوحدات 1/4000 من مساحة المخطط. |
| العرض | Int32 | يمثل عرض الشكل بوحدات 1/4000 من مساحة المخطط. |

### قيمة الإرجاع

يعيد كائن Shape الذي يمثل كائن WordArt الجديد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // إضافة WordArt إلى المخطط
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // تخصيص مظهر WordArt
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // احفظ المصنف
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


