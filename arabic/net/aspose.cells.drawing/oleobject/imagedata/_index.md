---
title: "OleObject.ImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تمثل صورة كائن ole كمصفوفة بايت"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

يمثل صورة كائن OLE كمصفوفة بايت.

```csharp
public byte[] ImageData { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // قراءة ملف الصورة إلى مصفوفة بايت
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // إضافة كائن OLE مع بيانات الصورة
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // تعيين خصائص الكائن المضمّن
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // عرض استخدام خاصية ImageData
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // احفظ المصنف
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


