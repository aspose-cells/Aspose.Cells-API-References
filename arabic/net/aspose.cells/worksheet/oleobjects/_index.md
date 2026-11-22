---
title: "Worksheet.OleObjects"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل مجموعة من OleObject في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

تمثل مجموعة من [`OleObject`](../../../aspose.cells.drawing/oleobject/) في ورقة العمل.

```csharp
public OleObjectCollection OleObjects { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة OleObject إلى ورقة العمل
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // تعديل خصائص OleObject
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // احفظ المصنف
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


