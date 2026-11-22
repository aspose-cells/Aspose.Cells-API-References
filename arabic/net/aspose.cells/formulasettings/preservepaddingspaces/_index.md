---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كان يجب الحفاظ على تلك المسافات وفواصل الأسطر التي تم تعبئتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

يشير إلى ما إذا كان يجب الحفاظ على تلك الفراغات وفواصل الأسطر التي تُملأ بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### ملاحظات

عادةً ما تكون تلك المسافات وفواصل الأسطر لأغراض بصرية فقط، ولا يؤثر الحفاظ عليها أو عدمه على النتيجة المحسوبة. من منظور الأداء، إذا لم تكن هناك متطلبات خاصة، فمن الأفضل عدم الحفاظ عليها أثناء معالجة الصيغ.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين صيغة مع مسافات التعبئة
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // السلوك الافتراضي (PreservePaddingSpaces هو true)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // تغيير الإعداد لإزالة مسافات التعبئة
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // احفظ المصنف
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


