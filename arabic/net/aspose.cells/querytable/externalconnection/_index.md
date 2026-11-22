---
title: "QueryTable.ExternalConnection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTable. يحصل على الاتصال الخارجي المرتبط"
type: docs
url: /ar/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

يحصل على الاتصال الخارجي المرتبط.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // الوصول إلى خاصية ExternalConnection (للقراءة فقط)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // عرض معلومات حول الاتصال الخارجي
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // عرض خصائص أخرى لجدول الاستعلام للسياق
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // احفظ المصنف
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


