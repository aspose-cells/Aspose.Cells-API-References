---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. الحصول على نص تسمية Grand Total في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

يحصل على نص التسمية "Grand Total" في جدول المحور.

```csharp
public override string GetTextOfGrandTotal()
```

### قيمة الإرجاع

نص تسمية "Grand Total"

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد (فقط للسياق)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // كائن من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // تغيير النص الافتراضي "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // استرجاع النص الحالي "Grand Total"
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // حفظ المصنف (لم يتم إنشاء PivotTable، لكن تم حفظ الملف لإثبات التنفيذ)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


