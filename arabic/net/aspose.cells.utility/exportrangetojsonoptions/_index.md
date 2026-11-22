---
title: "الفئة ExportRangeToJsonOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Utility.ExportRangeToJsonOptions. تشير إلى الخيارات التي تصدر النطاق إلى json"
type: docs
url: /ar/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

يشير إلى الخيارات التي تصدر النطاق إلى json.

```csharp
public class ExportRangeToJsonOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | يصدّر القيم النصية للخلايا إلى JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | يشير إلى ما إذا كان النطاق يحتوي على صف رأس. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | يشير إلى المسافة البادئة. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء خيارات التصدير
            var exportOptions = new ExportRangeToJsonOptions();
            
            // تصدير النطاق إلى JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // إخراج JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // حفظ إلى ملف (اختياري)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


