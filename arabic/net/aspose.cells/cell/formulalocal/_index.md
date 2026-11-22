---
title: "Cell.FormulaLocal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. احصل على الصيغة المهيأة حسب اللغة للخلية"
type: docs
url: /ar/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

احصل على الصيغة المنسقة حسب الإعداد المحلي للخلية.

```csharp
public string FormulaLocal { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن اللغة الافتراضية إلى الألمانية للتجربة
            workbook.Settings.Region = CountryCode.Germany;
            
            // الوصول إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            
            // عيّن الصيغة بالتنسيق القياسي (الإنجليزية)
            cell.Formula = "=SUM(B1:C1)";
            
            // اعرض الصيغ بالتنسيقين القياسي والمحلي
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // عيّن الصيغة بالتنسيق المحلي (الألمانية)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // اعرض الصيغ مرة أخرى لإظهار الفرق
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // وضح GetFormula مع التعريب
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


