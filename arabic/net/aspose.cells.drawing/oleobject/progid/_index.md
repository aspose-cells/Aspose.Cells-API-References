---
title: "OleObject.ProgID"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل أو تعين ProgID لكائن OLE"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

يحصل على أو يضبط ProgID لكائن OLE.

```csharp
public string ProgID { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة كائن OLE إلى ورقة العمل
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // تعيين ProgID لكائن OLE
            ole.ProgID = "AcroExch.Document.DC";
            
            // عرض ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // احفظ المصنف
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


