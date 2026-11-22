---
title: "WebQueryConnection.IsConsecutive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى ما إذا كان يجب معالجة الفواصل المتتالية كفاصل واحد فقط"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

علامة تشير إلى ما إذا كان يجب معالجة الفواصل المتتالية كفاصل واحد فقط.

```csharp
public bool IsConsecutive { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء اتصال استعلام ويب عن طريق الوصول إلى أول اتصال
            // (مع افتراض وجود اتصال واحد على الأقل متاح)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // عرض قيمة IsConsecutive الأولية (الافتراضية)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // تعيين IsConsecutive إلى true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // إعادة تعيين IsConsecutive إلى false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // حفظ المصنف مع اتصال استعلام الويب
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


