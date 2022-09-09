---
title: ImageType
second_title: Aspose.Cells لمرجع .NET API
description: يحصل على تنسيق صورة الصورة.
type: docs
weight: 60
url: /ar/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

يحصل على تنسيق صورة الصورة.

```csharp
public ImageType ImageType { get; }
```

### أمثلة

```csharp

[C#]
// إنشاء كائن مصنف
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// أدخل الصورة الأولى
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
// احصل على كائن الصورة المدرج
Picture pic1 = worksheet.Pictures[imgIndex1];
if(pic1.ImageType == Aspose.Cells.Drawing.ImageType.Png)
{
    // نوع الصورة هو png. ";
}
// أدخل الصورة الثانية
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
// احصل على كائن الصورة المدرج
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic2.ImageType == Aspose.Cells.Drawing.ImageType.Jpeg)
{
    // نوع الصورة هو jpg. ";
}
```

### أنظر أيضا

* enum [ImageType](../../imagetype)
* class [Picture](../../picture)
* مساحة الاسم [Aspose.Cells.Drawing](../../picture)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->