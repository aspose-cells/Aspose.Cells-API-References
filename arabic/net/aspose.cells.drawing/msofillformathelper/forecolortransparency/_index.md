---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormatHelper. تُرجع أو تضبط درجة لون المقدمة للملء المحدد كقيمة من 0.0 معتم إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

إرجاع أو تعيين درجة اللون الأمامي للملء المحدد كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double ForeColorTransparency { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تسمية لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // أنشئ مثيلًا لـ MsoFillFormatHelper باستخدام الانعكاس (بدون مُنشئ عام)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // اعرض قيمة ForeColorTransparency الافتراضية
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // اضبط ForeColor و ForeColorTransparency جديدين
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // اعرض القيم المحدثة
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // أظهر قراءة قيمة الشفافية
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // احفظ المصنف لعرض التنفيذ الناجح
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


