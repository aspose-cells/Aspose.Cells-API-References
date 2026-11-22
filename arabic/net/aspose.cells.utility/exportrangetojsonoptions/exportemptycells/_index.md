---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportRangeToJsonOptions. تشير إلى ما إذا كان تصدير الخلايا الفارغة كقيمة null"
type: docs
url: /ar/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // اترك الخلية B2 فارغة عن قصد
            
            // إنشاء خيارات التصدير وتمكين تصدير الخلايا الفارغة
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // تصدير النطاق إلى JSON
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### انظر أيضًا

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


