---
title: "Workbook.IsDigitallySigned"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تشير إلى ما إذا كان هذا الجدول الإلكتروني موقّعًا رقمياً"
type: docs
url: /ar/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

يشير إلى ما إذا كان هذا الجدول موقعًا رقمياً.

```csharp
public bool IsDigitallySigned { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // تحميل دفتر عمل موقّع رقمياً
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // تحقق مما إذا كان المصنف موقعًا رقميًا
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // احفظ نسخة (سيتم الحفاظ على التوقيع)
                book.Save("SignedCopy.xlsx");
                
                // إزالة التوقيع الرقمي
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // تحقق من أن التوقيع قد أُزيل
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


