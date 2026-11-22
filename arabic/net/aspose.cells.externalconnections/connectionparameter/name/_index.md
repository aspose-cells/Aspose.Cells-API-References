---
title: "ConnectionParameter.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. اسم المعامل"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

اسم المعلمة.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
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

                // للتوضيح، سنظهر كيف سيتم استخدام Name إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة Name الحالية واعرضها
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // تعيين قيمة Name جديدة (نظرًا لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // احفظ المصنف
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


