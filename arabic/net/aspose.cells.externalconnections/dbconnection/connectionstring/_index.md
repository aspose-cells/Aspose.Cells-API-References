---
title: "DBConnection.ConnectionString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تُستخدم سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;

                // إنشاء DBConnection جديد عن طريق إضافته إلى المجموعة
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // عرض قيمة ConnectionString الأولية
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // تعيين سلسلة اتصال جديدة
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // عرض قيمة ConnectionString المحدثة
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // احفظ المصنف
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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


