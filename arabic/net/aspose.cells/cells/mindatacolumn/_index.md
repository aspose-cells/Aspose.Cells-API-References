---
title: "Cells.MinDataColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأدنى لفهرس العمود للخلية التي تحتوي على بيانات"
type: docs
url: /ar/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

الحد الأدنى لفهرس العمود للخلية التي تحتوي على بيانات.

```csharp
public int MinDataColumn { get; }
```

### ملاحظات

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // أضف بعض البيانات إلى الخلايا (بدءًا من العمود 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // احصل على الحد الأدنى لمؤشر العمود الذي يحتوي على بيانات
            int minDataColumn = cells.MinDataColumn;
            
            // أخرج النتيجة.
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


