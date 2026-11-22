---
title: "فئة MsoFormatPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.MsoFormatPicture. تمثل تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

يمثل تنسيق الصورة.

```csharp
public class MsoFormatPicture
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | يمثل موضع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | يمثل موضع الجزء السفلي من مستطيل القص، بوحدة البوصة. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | يمثل تعديل السطوع للصورة بوحدة النسبة المئوية. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | يمثل تعديل التباين للصورة بوحدة النسبة المئوية. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | يمثل قيمة غاما للصورة. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | يشير إلى ما إذا كان يجب عرض هذه الصورة بتدرج الرمادي. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | يمثل موضع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | يمثل موضع الجانب الأيسر من مستطيل القص، بوحدة البوصة. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | يمثل موضع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | يمثل موضع الجانب الأيمن من مستطيل القص، بوحدة البوصة. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | يمثل موضع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | يمثل موضع الجزء العلوي من مستطيل القص، بوحدة البوصة. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | يحصل ويضبط اللون الشفاف للصورة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | يحصل على رمز التجزئة. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPictureDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // الوصول إلى كائن MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // تعيين خصائص MsoFormatPicture
            formatPicture.TopCropInch = 0.5;
            formatPicture.BottomCropInch = 0.5;
            formatPicture.LeftCropInch = 0.5;
            formatPicture.RightCropInch = 0.5;
            formatPicture.Transparency = 0.5;
            formatPicture.Contrast = 0.8;
            formatPicture.Brightness = 0.6;
            formatPicture.Gamma = 1.0;
            formatPicture.IsBiLevel = false;
            formatPicture.IsGray = false;

            // تعيين اللون الشفاف
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // احفظ المصنف
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


