---
title: "Validation.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. نسخ التحقق"
type: docs
url: /ar/net/aspose.cells/validation/copy/
---
## Validation.Copy method

نسخ التحقق.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | التحقق | التحقق المصدر. |
| copyOption | CopyOptions | خيار النسخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر مع بيانات نموذجية والتحقق
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // إضافة تحقق نموذجي إلى ورقة المصدر
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // إنشاء CellArea مع StartRow، StartColumn، EndRow، EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // إضافة تحقق إلى ورقة الوجهة (سيتم استبداله بالنسخ)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // عرض طريقة Copy مع CopyOptions
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // تحقق من أن التحقق تم نسخه بشكل صحيح
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


