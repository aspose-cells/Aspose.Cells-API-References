---
title: "WebQueryConnection.HtmlFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. كيفية التعامل مع التنسيق من مصدر HTML عند جلب بيانات استعلام الويب إلى ورقة العمل. ذات صلة عندما تكون sourceData هي True"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

كيفية معالجة التنسيق من مصدر HTML عند جلب بيانات استعلام الويب إلى ورقة العمل. ذو صلة عندما تكون sourceData صحيحة.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى أول اتصال استعلام ويب موجود (إن وجد)
            // أو إنشاء واحد جديد بتحميل ملف يحتوي على اتصالات ويب
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // عرض قيمة HtmlFormat الأولية
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // تعيين HtmlFormat إلى Rtf (للتوضيح عملية الكتابة)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // تعيين HtmlFormat إلى None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // حفظ المصنف مع اتصال استعلام الويب
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### انظر أيضًا

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


