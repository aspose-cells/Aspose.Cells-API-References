---
title: "الفئة CellsException"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellsException. الاستثناء الذي يُرمى عندما يحدث خطأ محدد في Aspose.Cells"
type: docs
url: /ar/net/aspose.cells/cellsexception/
---
## CellsException class

الاستثناء الذي يُرمى عندما يحدث خطأ محدد في Aspose.Cells.

```csharp
public class CellsException : ApplicationException
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | يمثل رمز استثناء مخصص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;
    using System.Collections;

    public class CellsExceptionDemo
    {
        public static void CellsExceptionExample()
        {
            try
            {
                // حاكي عملية تتسبب في استثناء
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // إحداث استثناء عن قصد عبر الوصول إلى خلية غير صالحة
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // معالجة CellsException
                Console.WriteLine("Aspose.Cells.CellsException caught!");
                Console.WriteLine($"Code: {ex.Code}");
                Console.WriteLine($"Message: {ex.Message}");
                Console.WriteLine($"TargetSite: {ex.TargetSite}");
                Console.WriteLine($"StackTrace: {ex.StackTrace}");
                Console.WriteLine($"HelpLink: {ex.HelpLink}");
                Console.WriteLine($"Source: {ex.Source}");
                Console.WriteLine($"HResult: {ex.HResult}");
                if (ex.InnerException != null)
                {
                    Console.WriteLine($"InnerException: {ex.InnerException.Message}");
                }
                foreach (DictionaryEntry entry in ex.Data)
                {
                    Console.WriteLine($"Data: {entry.Key} = {entry.Value}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


