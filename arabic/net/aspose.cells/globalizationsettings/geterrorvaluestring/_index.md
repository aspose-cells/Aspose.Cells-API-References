---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على قيمة السلسلة المعروضة لقيمة خطأ الخلايا"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

يحصل على قيمة النص المعروض لقيمة خطأ الخلية

```csharp
public virtual string GetErrorValueString(string err)
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

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين إعدادات العولمة المخصصة
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // إنشاء سيناريو خطأ: القسمة على الصفر
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // تعيينات قيم الأخطاء المخصصة
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


