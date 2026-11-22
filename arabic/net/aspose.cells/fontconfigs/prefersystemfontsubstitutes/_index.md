---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontConfigs. تشير إلى ما إذا كان يجب استخدام بدائل الخطوط النظامية أولاً أم لا عندما لا يتوفر الخط ولا يتم تعيين بديل لهذا الخط. مثال: على أوبونتو يتم عادة استبدال خط Arial بخط Liberation Sans. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

حدد ما إذا كان يجب استخدام بدائل الخطوط النظامية أولاً أم لا عندما لا يتوفر الخط ولا يتم تعيين بديل لهذا الخط. مثال: على أوبونتو، يتم عادةً استبدال الخط "Arial" بـ "Liberation Sans". القيمة الافتراضية هي false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض قيمة PreferSystemFontSubstitutes الحالية
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // تعيين PreferSystemFontSubstitutes إلى true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // إنشاء خلية بخط قد يحتاج إلى استبدال
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // حفظ المصنف لرؤية تأثيرات استبدال الخط
            workbook.Save("FontSubstitutionDemo.xlsx");

            // إعادة الضبط إلى القيمة الافتراضية
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


