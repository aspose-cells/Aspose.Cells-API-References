---
title: "SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص رأس حقل منطقة القيمة في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

يحصل على نص رأس حقل منطقة القيمة في جدول المحور.

```csharp
public override string GetTextOfDataFieldHeader()
```

### قيمة الإرجاع

نص اسم رأس حقل البيانات

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
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
                // احصل على النص الافتراضي لرأس حقل البيانات
                string dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {dataFieldHeaderText}");

                // تعيين نص مخصص لرأس حقل البيانات
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Updated data field header text: {dataFieldHeaderText}");

                // احفظ المصنف
                workbook.Save("GetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("GetTextOfDataFieldHeader method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


