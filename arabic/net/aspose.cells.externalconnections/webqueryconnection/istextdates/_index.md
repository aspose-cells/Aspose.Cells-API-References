---
title: "WebQueryConnection.IsTextDates"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى ما إذا كان يجب استيراد التواريخ إلى خلايا ورقة العمل كنص بدلاً من تواريخ"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

علامة تشير إلى ما إذا كان يجب استيراد التواريخ إلى خلايا ورقة العمل كنص بدلاً من تواريخ.

```csharp
public bool IsTextDates { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];
                
                // أنشئ اتصال استعلام ويب بتحميله من ملف موجود
                // أو بالوصول إلى اتصال موجود
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // اعرض القيمة الأولية لـ IsTextDates
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // اضبط IsTextDates على true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // أعد ضبط IsTextDates إلى false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // حفظ المصنف مع اتصال استعلام الويب
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
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


