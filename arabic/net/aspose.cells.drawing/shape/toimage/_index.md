---
title: "Shape.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تنشئ صورة الشكل وتحفظها إلى تدفق بالتنسيق المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageType) {#toimage_1}

ينشئ صورة الشكل ويحفظها إلى تدفق بالتنسيق المحدد.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج. |
| imageType | ImageType | النوع الذي سيتم حفظ الصورة به. |

### ملاحظات

الصيغ التالية مدعومة: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل عينة مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // تحويل الشكل إلى تدفق صورة
            using (MemoryStream imageStream = new MemoryStream())
            {
                shape.ToImage(imageStream, ImageType.Png);
                Console.WriteLine("Shape converted to image stream successfully");
            }
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_3}

يحفظ الشكل إلى ملف.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // تعيين خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // حفظ الشكل كصورة
            shape.ToImage("shape_image.png", options);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

يحفظ الشكل إلى تدفق.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### أمثلة

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage(imageStream, op);
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

يرجع كائن bitmap للشكل.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### أمثلة

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
System.Drawing.Bitmap btm = shape.ToImage(op);
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


