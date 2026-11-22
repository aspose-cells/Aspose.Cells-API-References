---
title: "Picture.DisplayAsIcon"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. صحيحة إذا تم عرض الكائن المحدد كأيقونة ولن يتم تغيير الصورة تلقائيًا"
type: docs
url: /ar/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

صحيح إذا تم عرض الكائن المحدد كأيقونة ولن يتم تغيير الصورة تلقائيًا.

```csharp
public bool DisplayAsIcon { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // عيّن خاصية DisplayAsIcon إلى true
            picture.DisplayAsIcon = true;
            
            // عيّن خصائص الصورة الأخرى
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // احفظ المصنف
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


