---
title: "WebQueryConnection.IsXml"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. true إذا كان مصدر استعلام الويب هو XML مقابل HTML وإلا false"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true إذا كان مصدر الاستعلام الويب هو XML (مقابل HTML)، وإلا false.

```csharp
public bool IsXml { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال بيانات (مع افتراض أنه WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // عرض قيمة IsXml الأولية
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // تعيين IsXml إلى true (نظرًا لأنه قابل للقراءة والكتابة)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // إعادة تعيين IsXml إلى false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


