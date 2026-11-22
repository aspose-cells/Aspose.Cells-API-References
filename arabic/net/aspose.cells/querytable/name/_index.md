---
title: "QueryTable.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTable. يحصل على اسم querytable"
type: docs
url: /ar/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

يحصل على اسم querytable.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمحاكاة جدول استعلام
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // تحقق مما إذا كان هناك أي جداول استعلام في ورقة العمل
                if (worksheet.QueryTables.Count > 0)
                {
                    // احصل على أول جدول استعلام
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // عرض قيمة الخاصية Name (عملية للقراءة فقط)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // عرض خصائص أخرى للقراءة فقط للسياق
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // احفظ المصنف
                workbook.Save("QueryTableNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


