---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. يحصل على قيمة السلسلة المعروضة لقيمة الخطأ في الخلايا"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

يحصل على قيمة النص المعروض لقيمة خطأ الخلية

```csharp
public override string GetErrorValueString(string err)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خطأ | String | قيم الأخطاء مثل #VALUE!,#NAME؟ |

### قيمة الإرجاع

بشكل افتراضي تُعيد قيمة الخطأ نفسها

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // إنشاء خلية بقيمة خطأ
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // استدعِ GetErrorValueString مع سلسلة قيمة الخطأ
                string errorString = settings.GetErrorValueString("#N/A");
                
                // اعرض النتيجة
                Console.WriteLine("Error value string: " + errorString);

                // أظهر التأثير عن طريق ضبط قيمة خلية أخرى إلى السلسلة المعادة
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


