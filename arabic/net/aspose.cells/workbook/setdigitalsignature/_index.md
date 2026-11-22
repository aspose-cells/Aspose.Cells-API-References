---
title: "Workbook.SetDigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تُعيّن توقيعًا رقميًا لملف جدول بيانات Excel2007 وما بعده"
type: docs
url: /ar/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

يحدد توقيعًا رقميًا لملف ورقة إلكترونية (Excel2007 وما بعده).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### ملاحظات

يدعم فقط إضافة توقيع رقمي Xmldsig

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // مسار دليل المصدر
            string sourceDir = "SourceDirectory/";
            
            // مسار دليل الإخراج
            string outputDir = "OutputDirectory/";

            // حمّل المصنف
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // إنشاء مجموعة توقيع رقمي
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // تحميل ملف الشهادة
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // إنشاء توقيع رقمي
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // إضافة توقيع إلى المجموعة
            digitalSignatures.Add(signature);

            // تعيين توقيع رقمي لدفتر العمل
            workbook.SetDigitalSignature(digitalSignatures);

            // احفظ المصنف
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


