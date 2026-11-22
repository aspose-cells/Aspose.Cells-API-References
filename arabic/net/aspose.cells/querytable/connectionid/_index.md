---
title: "QueryTable.ConnectionId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTable. يحصل على معرف الاتصال لجدول الاستعلام"
type: docs
url: /ar/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

يحصل على معرف الاتصال لجدول الاستعلام.

```csharp
public int ConnectionId { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمحاكاة سيناريو جدول الاستعلام
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // تحقق مما إذا كان هناك أي جداول استعلام في ورقة العمل
                if (worksheet.QueryTables.Count > 0)
                {
                    // احصل على أول جدول استعلام
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // عرض قيمة خاصية ConnectionId (للقراءة فقط)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // عرض خصائص أخرى ذات صلة للسياق
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // احفظ المصنف
                workbook.Save("ConnectionIdDemo.xlsx");
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


