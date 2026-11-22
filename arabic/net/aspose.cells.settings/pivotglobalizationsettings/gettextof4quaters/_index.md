---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotGlobalizationSettings. تحصل على النص المحلي لـ 4 أرباع"
type: docs
url: /ar/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

يحصل على النص المحلي لـ 4 أرباع.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetTextOf4Quarters(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء فئة إعدادات عولمة مخصصة ترث من PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // استدعِ طريقة GetTextOf4Quaters
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // إخراج أسماء الأرباع إلى وحدة التحكم
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // إضافة أسماء الأرباع إلى ورقة العمل
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // تنفيذ مخصص لـ PivotGlobalizationSettings لتجاوز GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // إرجاع أسماء أرباع مخصصة
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### انظر أيضًا

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


