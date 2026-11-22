---
title: "DataModelConnection.ConnectionString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelConnection. تُستخدم سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء مثيل DataModelConnection باستخدام كائن غير مهيأ
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // عرض قيمة ConnectionString الأولية (فارغ)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // ضبط خاصية ConnectionString
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // عرض قيمة ConnectionString المحدثة
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // ضبط الخصائص المطلوبة الأخرى لاتصال كامل
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // حفظ دفتر العمل مع الاتصال
                workbook.Save("ConnectionStringDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


