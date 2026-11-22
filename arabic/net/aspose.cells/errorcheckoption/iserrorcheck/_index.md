---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ErrorCheckOption. تتحقق مما إذا كان نوع الخطأ المعطى سيُفحص"
type: docs
url: /ar/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

يتحقق مما إذا كان نوع الخطأ المعطى سيُفحص.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | يمكن فحص نوع الخطأ |

### قيمة الإرجاع

تُعيد true إذا كان نوع الخطأ المعطى سيُفحص (سيظهر مثلث أخضر للخلية إذا فشل الفحص).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // تكوين إعدادات فحص الأخطاء
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // إضافة نطاق لتطبيق هذه الإعدادات
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // تحقق وعرض الإعدادات
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### انظر أيضًا

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


