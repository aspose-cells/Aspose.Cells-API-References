---
title: "WebQueryConnection.IsParsePre"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى ما إذا كان يتم تحليل البيانات الموجودة داخل وسوم HTML PRE في صفحة الويب إلى أعمدة عند استيراد الصفحة إلى جدول استعلام"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

علامة تشير إلى ما إذا كانت البيانات الموجودة داخل وسوم HTML PRE في صفحة الويب تُحلل إلى أعمدة عند استيراد الصفحة إلى جدول استعلام.

```csharp
public bool IsParsePre { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء اتصال استعلام ويب جديد باستخدام الاتصال الموجود من المصنف
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // عرض قيمة IsParsePre الأولية (الافتراضية)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // تعيين IsParsePre إلى true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // إعادة تعيين IsParsePre إلى false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // احفظ المصنف
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


