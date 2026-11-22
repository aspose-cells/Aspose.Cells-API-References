---
title: "Cell.ToJson"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحويل Cell إلى بيانات هيكل JSON"
type: docs
url: /ar/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

تحويل [`Cell`](../) إلى بيانات هيكل JSON.

```csharp
public string ToJson()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين بيانات عينة والأنماط
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // الحصول على الخلية وتحويلها إلى JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // إخراج JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


