---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomRenderSettings. تحدد عرض حد الخلية وفقًا لنوع الحد"
type: docs
url: /ar/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

يحدد عرض حد الخلية وفقًا لنوع الحد.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | CellBorderType | نوع حد الخلية |

### قيمة الإرجاع

عرض حد الخلية

### ملاحظات

سيتم تجاهل أي قيمة سالبة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء كائن من CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // استدعاء GetCellBorderWidth بأنواع حدود مختلفة
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // عرض النتائج
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // احفظ المصنف
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


