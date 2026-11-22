---
title: "OleObject.DisplayAsIcon"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. صحيحة إذا تم عرض الكائن المحدد كأيقونة ولن يتم تغيير الصورة تلقائيًا"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

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
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف كائن OLE (PDF) إلى ورقة العمل
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // احصل على كائن OLE
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // وضح خاصية DisplayAsIcon
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // إظهار المحتوى إذا أمكن
            
            // احفظ المصنف
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


