---
title: "Picture.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Picture. انسخ الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

انسخ الصورة.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | صورة | الصورة المصدر. |
| خيارات | CopyOptions | خيارات النسخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أدرج الصورة الأولى (باستخدام مسار صورة تجريبي)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // أدرج الصورة الثانية (باستخدام مسار صورة تجريبي)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // انسخ الصورة 1 إلى الصورة 2 باستخدام CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


