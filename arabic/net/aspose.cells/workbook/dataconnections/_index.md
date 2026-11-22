---
title: "Workbook.DataConnections"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على مجموعة ExternalConnection"
type: docs
url: /ar/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

تحصل على مجموعة [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/).

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // الوصول إلى خاصية DataConnections
                var dataConnections = workbook.DataConnections;

                // عرض القيمة الحالية للخاصية (عملية قراءة)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // التكرار عبر الاتصالات إذا وجدت أي منها
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("DataConnections has been demonstrated");

                // حفظ النتيجة
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


