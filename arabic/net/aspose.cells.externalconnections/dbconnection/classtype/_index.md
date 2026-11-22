---
title: "DBConnection.ClassType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تحصل على نوع كائن ExternalConnection هذا"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

يحصل على نوع هذا الكائن [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء كائن DBConnection جديد بإضافته إلى المجموعة
                // نظرًا لعدم وجود مُنشئ عام بدون معلمات في DBConnection،
                // سندع المجموعة تنشئه لنا
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // عرض قيمة ClassType (خاصية للقراءة فقط)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // إظهار ضبط خصائص أخرى لجعل المثال أكثر معنى
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // احفظ المصنف
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


