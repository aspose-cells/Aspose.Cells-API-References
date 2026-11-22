---
title: "Workbook.AddDigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. يضيف توقيعًا رقميًا إلى ملف جدول بيانات OOXML Excel2007 وما بعده"
type: docs
url: /ar/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

يضيف توقيعًا رقميًا إلى ملف جدول بيانات OOXML (Excel2007 وما بعده).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### ملاحظات

يدعم فقط إضافة Xmldsig Digital Signature إلى ملف جدول بيانات OOXML

### أمثلة

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض البيانات التجريبية
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // تحميل الشهادة (استبدل بمسار الشهادة وكلمة المرور الخاصة بك)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // إنشاء توقيع رقمي
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // إنشاء مجموعة توقيع رقمي وإضافة التوقيع
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // إضافة توقيع رقمي إلى المصنف
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // احفظ المصنف
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


