---
title: "ConnectionParameter.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. نوع المعامل المستخدم. إذا كان parameterTypevalue فسيتم استخدام القيمة من boolean أو double أو integer أو string. في هذه الحالة يُتوقع تحديد أحد هذه الأنواع فقط"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

نوع المعامل المستخدم. إذا كان parameterType=value، فسيتم استخدام القيمة من boolean أو double أو integer أو string. في هذه الحالة، من المتوقع تحديد أحد {boolean, double, integer, or string} فقط.

```csharp
public ConnectionParameterType Type { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                
                // إنشاء معامل اتصال (محاكى لأن معلمات المُنشئ غير معروفة)
                ConnectionParameter parameter = null;
                
                // في سيناريو حقيقي، ستقوم بإنشاء المعامل بشكل صحيح
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // للتوضيح، سنظهر كيف سيتم استخدام Type إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة Type الحالية واعرضها
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // تعيين قيمة Type جديدة (نظرًا لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


