---
title: "ConnectionParameter.CellReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. إشارة الخلية التي تحدد أي قيمة خلايا تُستخدم لمعلمة الاستعلام. تُستخدم فقط عندما يكون parameterType هو cell"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

مرجع الخلية الذي يشير إلى قيمة الخلية التي يجب استخدامها لمعلمة الاستعلام. يُستخدم فقط عندما يكون parameterType هو cell.

```csharp
public string CellReference { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // للتوضيح، سنظهر كيف سيتم استخدام CellReference إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة CellReference الحالية واعرضها
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // تعيين قيمة CellReference جديدة (نظرًا لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


