---
title: "ExternalConnection.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحصل على معرف الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

يحصل على معرف الاتصال.

```csharp
public int Id { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى أول اتصال خارجي (المصنف يأتي باتصالات افتراضية)
                ExternalConnection connection = workbook.DataConnections[0];

                // اعرض القيمة الحالية لـ Id (خاصية للقراءة فقط)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // عرض خصائص أخرى للقراءة فقط للسياق
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // احفظ المصنف
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


