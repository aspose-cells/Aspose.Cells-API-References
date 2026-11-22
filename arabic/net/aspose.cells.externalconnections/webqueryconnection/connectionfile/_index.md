---
title: "WebQueryConnection.ConnectionFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. يحصل على ملف الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

يحصل على ملف الاتصال.

```csharp
public override string ConnectionFile { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء ورقة عمل نموذجية تحتوي على بيانات استعلام ويب
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // الحصول على أول اتصال استعلام ويب موجود (إن وجد)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // عرض قيمة ConnectionFile (خاصية للقراءة فقط)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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


