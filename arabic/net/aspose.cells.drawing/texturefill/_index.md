---
title: "الفئة TextureFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.TextureFill. تغلف الكائن الذي يمثل تنسيق تعبئة النسيج"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

يغلف الكائن الذي يمثل تنسيق تعبئة النسيج

```csharp
public class TextureFill : Fill
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | يحصل ويضبط بيانات الصورة للتعبئة. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | يشير إلى ما إذا كان يتم تكرار الصورة كنقش. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | يحصل أو يضبط خيار تنسيق الصورة. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | يحصل ويضبط نوع تنسيق الصورة. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | يحصل على ويضبط مقياس تنسيق الصورة. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | يحصل على أو يضبط خيار تجانب الصورة. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | يحصل على ويضبط نوع النسيج |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(موروث من [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | الحصول على رمز التجزئة. (موروث من [`Fill`](../fill/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلاً مستطيلاً لتوضيح تعبئة النسيج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // طبق تعبئة النسيج على الشكل واحصل على كائن TextureFill الموجود
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // اضبط نوع النسيج المدمج
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // قم بتكوين خيارات التجانب
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // اضبط شفافية التعبئة والقياس
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // احفظ المصنف مع تطبيق تعبئة النسيج
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


