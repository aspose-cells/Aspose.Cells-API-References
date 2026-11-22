---
title: "VbaProject.CertRawData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. يحصل على البيانات الأولية للشهادة إذا تم توقيع مشروع VBA هذا"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

يحصل على البيانات الأولية للشهادة إذا كان مشروع VBA هذا موقعًا.

```csharp
public byte[] CertRawData { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع مشروع VBA
            Workbook workbook = new Workbook();
            // لا حاجة لإنشاء VbaProject جديد لأن المصنف يحتوي على واحد بالفعل

            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // التحقق مما إذا كان مشروع VBA موقعًا
            if (vbaProject.IsSigned)
            {
                // عرض البيانات الأولية للشهادة إذا تم التوقيع
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // مثال: حفظ بيانات الشهادة إلى ملف إذا كان موجودًا
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // سيناريو مثال: تحميل مصنف يحتوي على مشروع VBA موقع
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // احفظ المصنف
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


