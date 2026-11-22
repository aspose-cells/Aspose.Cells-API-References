---
title: "WebQueryConnection.IsXl97"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. هذه العلامة موجودة للتوافق مع الإصدارات القديمة من ملفات الجداول وتُضبط على true إذا تم إنشاء هذا الاستعلام الويب في Microsoft Excel 97. هذه سمة اختيارية يمكن تجاهلها"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

هذه العلامة موجودة لتوافقية مع ملفات الجداول الإلكترونية القديمة الموجودة، وتُضبط على true إذا تم إنشاء هذا الاستعلام الويب في Microsoft Excel 97. هذه خاصية اختيارية يمكن تجاهلها.

```csharp
public bool IsXl97 { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // أنشئ ورقة عمل تحتوي على بعض البيانات لجعل المثال ذا معنى
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // أنشئ اتصال استعلام ويب بتحميله من ملف موجود أو بإنشائه بشكل صحيح
                // نظرًا لأننا لا نستطيع إنشاء WebQueryConnection مباشرةً، سنصل إلى أحد الموجودين
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // اعرض القيمة الأولية لـ IsXl97
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // اضبط IsXl97 على true (نظرًا لأنه قابل للقراءة والكتابة)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // أعد ضبط IsXl97 إلى false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
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


