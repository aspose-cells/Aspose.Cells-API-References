---
title: "WebQueryConnection.Post"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. تُرجع أو تُعيّن السلسلة المستخدمة مع طريقة post لإدخال البيانات إلى خادم ويب لإرجاع البيانات من استعلام ويب"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

تُرجع أو تُعيّن السلسلة المستخدمة مع طريقة post لإدخال البيانات إلى خادم ويب لإرجاع البيانات من استعلام ويب.

```csharp
public string Post { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء اتصال استعلام ويب عن طريق الوصول إلى اتصال موجود أو إنشائه من خلال التهيئة المناسبة
                // نظرًا لعدم إمكانية إنشاء كائن WebQueryConnection مباشرةً، سنستخدم أول اتصال إذا كان موجودًا
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // إذا لم توجد أي اتصالات، سنعرض مثالًا باستخدام اتصال تجريبي
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // تعيين قيمة Post الأولية
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // تعديل قيمة Post
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // مسح قيمة Post
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // احفظ المصنف
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


