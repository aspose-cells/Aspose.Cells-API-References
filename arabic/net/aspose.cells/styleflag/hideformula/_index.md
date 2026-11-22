---
title: "StyleFlag.HideFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد إخفاء الصيغة"
type: docs
url: /ar/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

سيتم تطبيق إعداد إخفاء الصيغة.

```csharp
public bool HideFormula { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // إضافة صيغة إلى الخلية A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // إنشاء علامة نمط مع تعيين HideFormula إلى true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // إنشاء نمط وتعيين IsFormulaHidden إلى true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // تطبيق النمط على الخلية A1 باستخدام علامة النمط
            a1.SetStyle(style, styleFlag);

            // حماية ورقة العمل لرؤية تأثير HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // احفظ المصنف
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // تحقق من أن الصيغة مخفية
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


