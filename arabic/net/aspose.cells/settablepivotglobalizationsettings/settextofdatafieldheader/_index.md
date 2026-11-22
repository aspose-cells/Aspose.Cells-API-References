---
title: "SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تعيين نص عنوان حقل منطقة القيمة في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

يضبط نص عنوان حقل منطقة القيمة في PivotTable.

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص اسم رأس حقل البيانات |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // تعيين نص مخصص لرأس حقل البيانات
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // تحقق من التغيير عن طريق الحصول على النص الحالي
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // احفظ المصنف لعرض التنفيذ الناجح
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


