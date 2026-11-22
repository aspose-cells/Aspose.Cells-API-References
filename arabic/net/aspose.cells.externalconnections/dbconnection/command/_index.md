---
title: "DBConnection.Command"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات.

```csharp
public override string Command { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;

                // العثور على أول DBConnection في المجموعة (إن وجد)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // عرض قيمة Command الحالية (عملية قراءة)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // توضيح ضبط Command (خاصية قراءة‑كتابة)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // احفظ المصنف
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


