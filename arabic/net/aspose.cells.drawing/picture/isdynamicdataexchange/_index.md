---
title: "Picture.IsDynamicDataExchange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل أو تضبط ما إذا كان تبادل البيانات الديناميكي"
type: docs
url: /ar/net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

يحصل على أو يضبط ما إذا كان هناك تبادل بيانات ديناميكي

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsDynamicDataExchangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // عرض خاصية IsDynamicDataExchange
            Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
            
            // عيّن IsDynamicDataExchange إلى true
            picture.IsDynamicDataExchange = true;
            Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);

            // احفظ المصنف
            workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);

            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
            Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
            Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


