---
title: "OleObject.ObjectData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تمثّل بيانات كائن ole المدمجة كمصفوفة بايت"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

يمثل بيانات كائن OLE المضمنة كمصفوفة بايت.

```csharp
public byte[] ObjectData { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            var workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            var worksheet = workbook.Worksheets[0];
            
            // مسارات ملفات عينة (استبدلها بالمسارات الفعلية في بيئتك)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // أضف كائن OLE مع بيانات الصورة الأولية
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // عدّل بيانات كائن OLE
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // احفظ المصنف
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


