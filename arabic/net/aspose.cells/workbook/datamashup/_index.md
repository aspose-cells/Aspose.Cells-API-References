---
title: "Workbook.DataMashup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على بيانات الدمج"
type: docs
url: /ar/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

يحصل على بيانات الدمج.

```csharp
public DataMashup DataMashup { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات تجريبية لتفعيل Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // حفظ إلى ملف
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // إعادة فتح المصنف للوصول إلى DataMashup
            workbook = new Workbook(sourcePath);
            
            // الوصول إلى صيغ Power Query عبر خاصية DataMashup
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // إخراج المعلومات الأساسية حول الاستعلامات
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // إذا كان هناك أي استعلامات، اعرض تفاصيل الأول
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // حفظ إلى ملف جديد
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### انظر أيضًا

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


