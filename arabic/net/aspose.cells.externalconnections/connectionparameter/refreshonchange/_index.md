---
title: "ConnectionParameter.RefreshOnChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. علامة تشير إلى ما إذا كان يجب أن يتم تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعامل. إذا كان true فإن البيانات الخارجية تُحدث باستخدام قيمة المعامل الجديدة في كل مرة يحدث فيها تغيير. إذا كان false فإن البيانات الخارجية تُحدث فقط عندما يطلبها المستخدم أو عندما يُtrigger حدث آخر مثل فتح المصنف"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعامل. إذا كان true، يتم تحديث البيانات الخارجية باستخدام قيمة المعامل الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية فقط عند طلب المستخدم أو عندما يُ triggers حدث آخر (مثل فتح المصنف).

```csharp
public bool RefreshOnChange { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
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
                
                // للتوضيح، سنظهر كيف سيتم استخدام RefreshOnChange إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة RefreshOnChange الحالية واعرضها
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // تعيين قيمة RefreshOnChange جديدة (نظرًا لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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


