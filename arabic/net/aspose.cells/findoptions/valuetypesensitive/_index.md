---
title: "FindOptions.ValueTypeSensitive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. تشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون نفس المفتاح الذي تم البحث عنه"
type: docs
url: /ar/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون مطابقًا للمفتاح الذي تم البحث عنه.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف أنواع قيم مختلفة إلى الخلايا
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // إنشاء خيارات البحث مع ValueTypeSensitive = true
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // ابحث عن الرقم 100 (لن يجد السلسلة "100")
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // ابحث عن السلسلة "100" (لن يجد الرقم 100)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // غيّر إلى ValueTypeSensitive = false
            options.ValueTypeSensitive = false;
            
            // الآن كلا البحثين سيجدان أي خلية تحتوي على "100" أو 100
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


