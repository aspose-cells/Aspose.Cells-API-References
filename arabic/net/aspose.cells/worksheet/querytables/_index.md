---
title: "Worksheet.QueryTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على QueryTableCollection في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

تحصل على [`QueryTableCollection`](../../querytablecollection/) في ورقة العمل.

```csharp
public QueryTableCollection QueryTables { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // احصل على أول جدول استعلام (نظرًا لأننا لا نستطيع إضافة جداول جديدة مباشرةً)
            // ملاحظة: مجموعة QueryTables للقراءة فقط في إصدار API هذا
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // عرض معلومات جدول الاستعلام
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // احفظ المصنف
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


