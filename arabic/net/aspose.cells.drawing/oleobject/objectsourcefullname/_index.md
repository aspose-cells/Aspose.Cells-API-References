---
title: "OleObject.ObjectSourceFullName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تُرجع الاسم الكامل للمصدر للملف المصدر لكائن OLE المرتبط"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

يرجع الاسم الكامل للمصدر للملف المصدر لكائن OLE المرتبط.

```csharp
public string ObjectSourceFullName { get; set; }
```

### ملاحظات

يدعم فقط تعيين الاسم الكامل للمصدر عندما يكون نوع الملف OleFileType.Unknown. مثل ملفات wav ، avi .. إلخ

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة كائن OLE (باستخدام بيانات الملف كمصفوفة بايت)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // تعيين والحصول على ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // احفظ المصنف
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


