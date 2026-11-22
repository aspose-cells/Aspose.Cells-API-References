---
title: "Picture.IsSameSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Picture. تُرجع ما إذا كان الشكل هو نفسه"
type: docs
url: /ar/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

يرجع ما إذا كان الشكل متماثل.

```csharp
public override bool IsSameSetting(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أدرج الصورة الأولى (باستخدام مسار صورة تجريبي)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // أدرج الصورة الثانية (باستخدام مسار صورة تجريبي مختلف)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // قارن الصورة بنفسها
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // قارن بين الصور المختلفة
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


