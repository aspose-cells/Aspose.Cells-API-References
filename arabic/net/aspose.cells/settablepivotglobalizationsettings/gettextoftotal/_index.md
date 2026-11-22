---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص تسمية \"Total\" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

يحصل على نص تسمية "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات.

```csharp
public override string GetTextOfTotal()
```

### قيمة الإرجاع

نص تسمية "Total"

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات العينة للسياق
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // تعيين نص مخصص لتسمية "Total"
                settings.SetTextOfTotal("Custom Total");

                // احصل على نص تسمية "Total"
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // احفظ المصنف
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


