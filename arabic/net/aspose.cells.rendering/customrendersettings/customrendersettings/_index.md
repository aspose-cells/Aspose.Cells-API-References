---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ CustomRenderSettings. Ctor"
type: docs
url: /ar/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

منشئ.

```csharp
public CustomRenderSettings()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // إنشاء كائن من CustomRenderSettings باستخدام المُنشئ
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // عرض تأكيد استدعاء المُنشئ بنجاح
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // إظهار أن الكائن يعمل عن طريق استدعاء طريقة
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // احفظ المصنف
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


