---
title: "DataModelConnection.Command"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelConnection. السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات"
type: docs
url: /ar/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
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

                // عرض قيمة Command الأولية (فارغ)
                Console.WriteLine("Initial Command: " + connection.Command);

                // تعيين خاصية Command
                connection.Command = "SELECT * FROM Customers";
                
                // عرض قيمة Command المحدثة
                Console.WriteLine("Updated Command: " + connection.Command);

                // ضبط الخصائص المطلوبة الأخرى لاتصال كامل
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // حفظ دفتر العمل مع الاتصال
                workbook.Save("CommandDemo.xlsx");
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


