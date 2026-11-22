---
title: "WebQueryConnection.IsSameSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى ما إذا كان يجب تحليل جميع الجداول داخل كتلة PRE بنفس إعدادات العرض كما في الصف الأول"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

علامة تشير إلى ما إذا كان يجب تحليل جميع الجداول داخل كتلة PRE بنفس إعدادات العرض للصف الأول.

```csharp
public bool IsSameSettings { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال استعلام ويب موجود إذا كان متاحًا
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // عرض قيمة IsSameSettings الأولية
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // تعيين IsSameSettings إلى true (نظرًا لأنه قابل للقراءة والكتابة)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // إعادة تعيين IsSameSettings إلى false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


