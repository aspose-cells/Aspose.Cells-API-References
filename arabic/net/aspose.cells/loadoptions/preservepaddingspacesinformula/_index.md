---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تشير إلى ما إذا كان يجب الحفاظ على تلك الفراغات وفواصل الأسطر التي تم تعبئتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

يشير إلى ما إذا كان سيتم الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وضبطها. القيمة الافتراضية هي false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### ملاحظات

بعد تحميل دفتر العمل من ملف القالب باستخدام هذا الخيار، سيتم تعيين [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) إلى نفس القيمة مع هذه الخاصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تمكين الحفاظ على الفراغات المعبأة في الصيغ
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // الوصول إلى ورقة العمل الأولى وتعيين صيغة مع فراغات معبأة
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // حفظ وإعادة تحميل دفتر العمل باستخدام خيار PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // تحقق من أن الصيغة حافظت على الفراغات بعد إعادة التحميل
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


