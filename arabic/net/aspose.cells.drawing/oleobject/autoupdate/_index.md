---
title: "OleObject.AutoUpdate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحدد ما إذا كان الرابط إلى OleObject يتم تحديثه تلقائيًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

يحدد ما إذا كان الارتباط بـ OleObject يتم تحديثه تلقائيًا أم لا.

```csharp
public bool AutoUpdate { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء ملفات عينات للتوضيح
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // إنشاء ملف صورة عينة إذا لم يكن موجودًا
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // إنشاء ملف Excel عينة إذا لم يكن موجودًا
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // قراءة بيانات الصورة
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // إضافة OleObject إلى ورقة العمل
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // تعيين خصائص OleObject
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // عرض خاصية AutoUpdate
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // احفظ المصنف
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


