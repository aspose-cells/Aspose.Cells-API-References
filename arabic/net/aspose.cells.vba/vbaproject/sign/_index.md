---
title: "VbaProject.Sign"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProject. توقيع هذا المشروع VBA باستخدام DigitalSignature"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

وقّع مشروع VBA هذا باستخدام DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### أمثلة

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodSignWithDigitalSignatureDemo
    {
        public static void Run()
        {
            // حمّل دفتر العمل مع مشروع VBA
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // الحصول على مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // تحميل الشهادة من ملف
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // أنشئ توقيعًا رقميًا
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // توقيع مشروع VBA
                vbaProject.Sign(certSign);
                
                // حفظ المصنف الموقّع
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // تحقق من التوقيع
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


