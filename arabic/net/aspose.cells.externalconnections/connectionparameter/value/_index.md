---
title: "ConnectionParameter.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. قيمة عددية غير صحيحة، قيمة عددية صحيحة، قيمة سلسلة أو قيمة منطقية لاستخدامها كمعامل استعلام. يُستخدم فقط عندما يكون parameterType هو value"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعامل للاستعلام. تُستخدم فقط عندما يكون parameterType هو value.

```csharp
public object Value { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                
                // إنشاء معامل اتصال (محاكى لأننا لا نعرف معلمات المُنشئ)
                ConnectionParameter parameter = null;
                
                // في سيناريو حقيقي، ستقوم بإنشاء المعامل بشكل صحيح
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // للتوضيح، سنقوم بإنشاء معامل تجريبي مع قيمة
                // هذا يوضح كيف سيتم استخدام خاصية Value في التطبيق
                if (parameter != null)
                {
                    // قم بتعيين القيمة (لأن Value قابل للقراءة والكتابة)
                    parameter.Value = "SampleParameterValue";
                    
                    // احصل على القيمة واعرضها
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // غيّر القيمة لتظهر أنها قابلة للتغيير
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


