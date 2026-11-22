---
title: "Workbook.RemoveDigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. يزيل التوقيع الرقمي من هذا جدول البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

يزيل التوقيع الرقمي من هذه الورقة الإلكترونية.

```csharp
public void RemoveDigitalSignature()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على توقيع رقمي
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // حفظ مع توقيع رقمي (في السيناريو الحقيقي سيتم التوقيع خارجيًا)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // تحميل المصنف الموقّع
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // إزالة التوقيع الرقمي
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // تحقق من أن التوقيع قد أُزيل
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


