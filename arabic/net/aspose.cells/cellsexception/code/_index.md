---
title: "CellsException.Code"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsException. تمثل رمز الاستثناء المخصص"
type: docs
url: /ar/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

يمثل رمز استثناء مخصص.

```csharp
public ExceptionType Code { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsExceptionPropertyCodeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف ومحاولة الوصول إلى ورقة عمل غير موجودة
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // عرض كيفية استخدام خاصية Code
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


