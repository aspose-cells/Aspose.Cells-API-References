---
title: "ExternalConnection.RefreshOnLoad"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. true إذا كان يجب تحديث هذا الاتصال عند فتح الملف وإلا false"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ.

```csharp
public bool RefreshOnLoad { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (المصنف يأتي باتصالات افتراضية)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض القيمة الأولية لـ RefreshOnLoad
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // إظهار تعيين الخاصية (نظرًا لأنها قابلة للقراءة والكتابة).
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("RefreshOnLoadDemo.xlsx");
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


