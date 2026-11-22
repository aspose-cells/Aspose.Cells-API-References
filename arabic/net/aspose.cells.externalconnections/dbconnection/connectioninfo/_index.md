---
title: "DBConnection.ConnectionInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تُستخدم سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.ConnectionString. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionInfoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // إنشاء كائن DBConnection جديد بإضافته إلى المجموعة
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // إعداد اتصال أساسي لإظهار خاصية ConnectionInfo
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // عرض القيمة الحالية لخاصية ConnectionInfo
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // نظرًا لأن ConnectionInfo ليست للقراءة فقط، إظهار ضبطها
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // احفظ المصنف
                workbook.Save("ConnectionInfoDemo.xlsx");

                Console.WriteLine("ConnectionInfo demonstration completed successfully.");
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


