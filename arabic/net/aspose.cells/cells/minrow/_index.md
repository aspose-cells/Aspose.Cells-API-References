---
title: "Cells.MinRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأدنى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط"
type: docs
url: /ar/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط.

```csharp
public int MinRow { get; }
```

### ملاحظات

تحتاج هذه الخاصية إلى التكرار والتحقق من الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ويجب عدم استدعائها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بعض البيانات لتوضيح MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // اعرض معلومات MinRow
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // امسح المحتويات بدءًا من MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // تحقق من المسح عن طريق فحص ما إذا كانت الخلايا فارغة
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


