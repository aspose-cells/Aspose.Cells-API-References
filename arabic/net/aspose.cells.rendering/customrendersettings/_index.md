---
title: "الفئة CustomRenderSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.CustomRenderSettings. تمثل إعدادات مخصصة أثناء العرض"
type: docs
url: /ar/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

يمثل إعدادات مخصصة أثناء التصيير.

```csharp
public class CustomRenderSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | منشئ. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | يحدد عرض حد الخلية وفقًا لنوع الحد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // إنشاء مثال من CustomRenderSettings باستخدام المنشئ الافتراضي
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // عرض طريقة GetCellBorderWidth مع أنواع حدود مختلفة
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // عرض النتائج
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // احفظ المصنف
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


