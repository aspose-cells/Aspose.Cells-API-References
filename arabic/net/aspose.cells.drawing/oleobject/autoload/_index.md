---
title: "OleObject.AutoLoad"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحدد ما إذا كان يجب استدعاء تطبيق المضيف للكائن المضمن لتحميل بيانات الكائن تلقائيًا عند فتح دفتر العمل الأصلي."
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

يحدد ما إذا كان يجب استدعاء تطبيق المضيف للكائن المضمّن لتحميل بيانات الكائن تلقائيًا عند فتح دفتر العمل الأصلي.

```csharp
public bool AutoLoad { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة OleObject إلى ورقة العمل
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // تعيين خصائص OleObject
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // عرض خاصية AutoLoad
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // احفظ المصنف
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


