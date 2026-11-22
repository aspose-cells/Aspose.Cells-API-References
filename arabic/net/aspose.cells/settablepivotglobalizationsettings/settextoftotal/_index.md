---
title: "SettablePivotGlobalizationSettings.SetTextOfTotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تعيين نص تسمية Total في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

يضبط نص تسمية "Total" في PivotTable.

```csharp
public void SetTextOfTotal(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص مخصص |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات العينة للسياق
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // الحصول على النص الافتراضي "Total"
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // تعيين نص مخصص لـ "Total"
                settings.SetTextOfTotal("Custom Total Label");

                // تحقق من التغيير
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // احفظ المصنف
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


