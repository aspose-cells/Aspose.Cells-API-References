---
title: "التعداد PasteOperationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.PasteOperationType. يمثل نوع العملية عند لصق نطاق"
type: docs
url: /ar/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

يمثل نوع العملية عند لصق نطاق.

```csharp
public enum PasteOperationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا عملية. |
| Add | `1` | إضافة |
| Subtract | `2` | طرح |
| Multiply | `3` | ضرب |
| Divide | `4` | قسمة |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // أنشئ خيارات اللصق باستخدام PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // أنشئ نطاقًا وانسخه باستخدام خيارات اللصق
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // احفظ المصنف
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


