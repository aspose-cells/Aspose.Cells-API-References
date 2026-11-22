---
title: "MsoFillFormatHelper.BackColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormatHelper. يحصل على ويضبط لون الخلفية للملف"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

يحصل ويضبط لون الخلفية للملف.

```csharp
public Color BackColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تسمية فقط لإضافة بعض المحتوى في الورقة
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper لا يُظهر مُنشئًا عامًا، استخدم الانعكاس لإنشائه
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // اضبط BackColor إلى لون معروف (مثال: LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // اقرأ قيمة BackColor وعرضها
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // اختياريًا يمكنك أيضًا قراءة ForeColor لإظهار أنه يبقى افتراضيًا
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // احفظ المصنف – fill helper غير مرتبط بشكل,
                // لكن الحفظ يُظهر أن الشيفرة تم تشغيلها دون خطأ.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


