---
title: "ExternalConnection.OdcFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد المسار الكامل لملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل اتصال أثناء محاولة تحديث البيانات وإعادة الاتصال reconnectionMethod1، فإن تطبيق الجداول سيحاول مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المدمج داخل المصنف."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجدول الإلكتروني مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن داخل دفتر العمل.

```csharp
public string OdcFile { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عرض قيمة OdcFile الحالية.
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // تعيين قيمة OdcFile جديدة (نظرًا لأنها قابلة للقراءة والكتابة).
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // مسح قيمة OdcFile.
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("OdcFileDemo.xlsx");
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


