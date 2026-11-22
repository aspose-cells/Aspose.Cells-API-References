---
title: "ExternalConnection.KeepAlive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. True عندما يجب على تطبيق الجداول الإلكترونية بذل جهود للحفاظ على فتح الاتصال. عندما يكون false يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

true عندما يجب على تطبيق الجدول الإلكتروني بذل الجهود للحفاظ على الاتصال مفتوحًا. عندما يكون false، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات.

```csharp
public bool KeepAlive { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عرض قيمة KeepAlive الحالية
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // تبديل قيمة KeepAlive لأنها قابلة للقراءة والكتابة
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("KeepAliveDemo.xlsx");
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


