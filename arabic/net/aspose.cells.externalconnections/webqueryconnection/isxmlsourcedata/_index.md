---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى أنه يجب استيراد بيانات مصدر XML بدلاً من جدول HTML نفسه"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

علامة تشير إلى أنه يجب استيراد بيانات المصدر XML بدلاً من جدول HTML نفسه.

```csharp
public bool IsXmlSourceData { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى اتصال استعلام ويب موجود أو إنشاء واحد من خلال التهيئة المناسبة
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // عرض قيمة IsXmlSourceData الأولية
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // تعيين IsXmlSourceData إلى true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // إعادة تعيين IsXmlSourceData إلى false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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


