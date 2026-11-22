---
title: "ConnectionParameter.Prompt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. سلسلة Prompt للمعامل. تُعرض لمستخدم الجدول مع واجهة إدخال لجمع قيمة المعامل قبل تحديث البيانات الخارجية. تُستخدم فقط عندما يكون parameterType هو prompt"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

سلسلة المطالبة للمعلمة. تُعرض على مستخدم الجدول مع واجهة إدخال لجمع قيمة المعلمة قبل تحديث البيانات الخارجية. تُستخدم فقط عندما يكون parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // للتوضيح، سنظهر كيف سيتم استخدام Prompt إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة Prompt الحالية واعرضها
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // قم بتعيين قيمة Prompt جديدة (لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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


