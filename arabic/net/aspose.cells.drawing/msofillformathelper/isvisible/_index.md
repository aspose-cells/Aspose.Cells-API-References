---
title: "MsoFillFormatHelper.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormatHelper. تشير إلى ما إذا كان هناك تعبئة"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

يشير إلى ما إذا كان هناك ملء.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تسمية لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // أنشئ مثيلًا لـ MsoFillFormatHelper باستخدام الانعكاس (بدون مُنشئ عام)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // اعرض القيمة الافتراضية لـ IsVisible
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // عيّن IsVisible إلى true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // عيّن IsVisible إلى false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // اقرأ القيمة الحالية لـ IsVisible
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // احفظ المصنف لعرض التنفيذ الناجح
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


