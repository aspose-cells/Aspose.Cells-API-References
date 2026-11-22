---
title: "OleObject.IsAutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. True تشير إلى أن حجم كائن ole سيتغير تلقائيًا ليتطابق مع حجم لقطة المحتوى المدمج عند تفعيل كائن ole"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

صحيح يعني أن حجم كائن OLE سيتغير تلقائيًا ليتطابق مع حجم لقطة المحتوى المضمن عند تفعيل كائن OLE.

```csharp
public bool IsAutoSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة كائن OLE (باستخدام بيانات الملف كمصفوفة بايت)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // تعيين وعرض خاصية IsAutoSize
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // تغيير الخاصية
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // احفظ المصنف
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


