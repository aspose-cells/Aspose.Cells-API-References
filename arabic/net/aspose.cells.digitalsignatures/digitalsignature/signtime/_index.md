---
title: "DigitalSignature.SignTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DigitalSignature. الوقت الذي تم فيه توقيع المستند"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

الوقت الذي تم فيه توقيع المستند.

```csharp
public DateTime SignTime { get; set; }
```

### أمثلة

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertySignTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // إنشاء وإضافة توقيع رقمي
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // عرض خاصية SignTime
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // حفظ المصنف الموقّع
                workbook.Save("SignedWorkbook.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


