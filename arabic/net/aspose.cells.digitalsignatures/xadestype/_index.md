---
title: "تعداد XAdESType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DigitalSignatures.XAdESType. نوع توقيع XML المتقدم الإلكتروني XAdES"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

نوع توقيع إلكتروني متقدم XML (XAdES).

```csharp
public enum XAdESType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | XAdES غير مفعّل. |
| XAdES | `1` | XAdES الأساسي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;
    using System.Security.Cryptography.X509Certificates;

    public class XAdESTypeDemo
    {
        public static void XAdESTypeExample()
        {
            // دليل المصدر
            string sourceDir = "path_to_source_directory";
            // دليل الإخراج
            string outputDir = "path_to_output_directory";
            // حمّل المصنف
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // حدد كلمة المرور لملف PFX
            string password = "pfxPassword";
            // مسار ملف PFX
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // أنشئ توقيعًا رقميًا
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // حدد نوع XAdES
            signature.XAdESType = XAdESType.XAdES;

            // أنشئ مجموعة من التوقيعات الرقمية
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // عيّن التوقيع الرقمي للمصنف
            workbook.SetDigitalSignature(dsCollection);

            // احفظ المصنف مع التوقيع الرقمي
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // تحقق من التوقيع الرقمي
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
                Console.WriteLine($"XAdES Type: {ds.XAdESType}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


