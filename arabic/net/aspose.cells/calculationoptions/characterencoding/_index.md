---
title: "CalculationOptions.CharacterEncoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. يحدد الترميز المستخدم لتشفير/فك تشفير الأحرف عند حساب الصيغ. بالنسبة للدوال مثل CHAR CODE تعتمد النتيجة المحسوبة على إعدادات المنطقة ومجموعة الأحرف الافتراضية للبيئة. باستخدام هذه الخاصية يمكن للمستخدم تحديد الترميز المناسب لتلك الدوال للحصول على النتيجة المتوقعة"
type: docs
url: /ar/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

يحدد الترميز المستخدم لترميز/فك ترميز الأحرف عند حساب الصيغ. بالنسبة للدوال مثل CHAR و CODE، تعتمد النتيجة المحسوبة على إعدادات المنطقة ومجموعة الأحرف الافتراضية للبيئة. باستخدام هذه الخاصية يمكن للمستخدم تحديد الترميز المناسب لتلك الدوال للحصول على النتيجة المتوقعة.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


