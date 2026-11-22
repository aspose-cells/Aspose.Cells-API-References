---
title: "WebQueryConnection.ClassType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. يحصل على نوع كائن ExternalConnection هذا"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

يحصل على نوع هذا الكائن [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
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
                    // عرض قيمة ClassType (خاصية للقراءة فقط)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // تحقق من قيمة التعداد المتوقعة للاستعلام الويب
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


