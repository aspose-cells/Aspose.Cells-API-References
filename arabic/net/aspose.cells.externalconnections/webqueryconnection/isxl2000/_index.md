---
title: "WebQueryConnection.IsXl2000"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. هذه العلامة موجودة للتوافق مع الإصدارات القديمة من ملفات الجداول وتُضبط على true إذا تم تحديث هذا الاستعلام الويب في تطبيق جدول بيانات أحدث أو يساوي Microsoft Excel 2000. هذه سمة اختيارية يمكن تجاهلها"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

هذه العلامة موجودة لتوافقية مع ملفات الجداول الإلكترونية القديمة الموجودة، وتُضبط على true إذا تم تحديث هذا الاستعلام الويب في تطبيق جدول إلكتروني أحدث من أو يساوي Microsoft Excel 2000. هذه خاصية اختيارية يمكن تجاهلها.

```csharp
public bool IsXl2000 { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى أول اتصال استعلام ويب موجود (إن وجد)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // اعرض القيمة الأولية لـ IsXl2000
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // اضبط IsXl2000 على true (نظرًا لأنه قابل للقراءة والكتابة)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // أعد ضبط IsXl2000 إلى false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
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


