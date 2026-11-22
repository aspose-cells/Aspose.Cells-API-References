---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تعيين نص تسمية Multiple Items في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

يضبط نص تسمية "(Multiple Items)" في PivotTable.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات التجريبية (اختياري، فقط للسياق)
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
                // تعيين نص مخصص لتسمية "(Multiple Items)" في PivotTable
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // استرجاع وعرض النص المحدث
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (اختياري) حفظ المصنف – لا يلزم وجود PivotTable لهذا العرض التوضيحي
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


