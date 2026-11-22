---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على النص للاسم المحمي المحدد"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

يحصل على النص لاسم محمي محدد.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| protectedName | String | الاسم المحمي في PivotTable. |

### قيمة الإرجاع

الأسماء المحمية المحلية في PivotTable.

### ملاحظات

في برنامج Ms Excel، بعض الأسماء غير مسموح باستخدامها كاسم لحقول PivotFields في PivotTable. تختلف هذه الأسماء حسب المنطقة، ويمكن للمستخدم تحديدها صراحةً وفقًا للمنطقة المستخدمة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات العينة للسياق
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // تعيين نص مخصص لاسم محمي
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // احصل على نص الاسم المحمي
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // احفظ المصنف
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


