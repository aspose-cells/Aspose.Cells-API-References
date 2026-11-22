---
title: "الفئة TilePicOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.TilePicOption. تمثل صورة البلاط كنقش"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

يمثل صورة البلاط كنقش.

```csharp
public class TilePicOption
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TilePicOption](tilepicoption/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | يحصل أو يضبط المحاذاة للبلاط. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | يحصل أو يضبط نوع المرآة للبلاط. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | يحصل أو يضبط إزاحة X لصورة البلاط. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | يحصل أو يضبط إزاحة Y لصورة البلاط. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | يحصل أو يضبط مقياس X لصورة البلاط. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | يحصل أو يضبط مقياس Y لصورة البلاط. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مخطط للتوضيح
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // تعيين نوع التعبئة إلى نقش
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // تحميل صورة نموذجية (استبدل بالمسار الفعلي)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // إنشاء وتكوين TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // احفظ المصنف
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


