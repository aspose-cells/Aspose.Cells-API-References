---
title: "WebQueryConnection.IsHtmlTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. علامة تشير إلى ما إذا كان يجب أن تعمل استعلامات الويب فقط على جداول HTML"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/ishtmltables/
---
## WebQueryConnection.IsHtmlTables property

علامة تشير إلى ما إذا كان يجب أن تعمل استعلامات الويب فقط على جداول HTML.

```csharp
public bool IsHtmlTables { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsHtmlTablesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // إنشاء اتصال استعلام ويب عبر فهرس المجموعة
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

                Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
                
                connection.IsHtmlTables = true;
                Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);

                workbook.Save("IsHtmlTablesDemo.xlsx");
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


