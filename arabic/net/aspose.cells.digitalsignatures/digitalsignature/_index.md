---
title: "الفئة DigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DigitalSignatures.DigitalSignature. التوقيع في الملف"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

التوقيع في الملف.

```csharp
public class DigitalSignature
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | منشئ digitalSignature. يستخدم تنفيذ .Net. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | منشئ digitalSignature. يستخدم تنفيذ Bouncy Castle. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | كائن الشهادة الذي تم استخدامه لتوقيع المستند. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | الغرض من التوقيع. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | يحدد GUID يمكن الإشارة إليه عبره مع GUID لخط التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | إذا كان هذا التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، ستكون هذه القيمة true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | يحدد معرف الفئة لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | الوقت الذي تم فيه توقيع المستند. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | نوع XAdES. القيمة الافتراضية هي None (XAdES غير مفعل). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // إنشاء توقيع رقمي باستخدام منشئ الشهادة
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // عيّن الخصائص الإضافية
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // إضافة توقيع إلى المصنف
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // عرض معلومات التوقيع
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // حفظ المصنف الموقّع
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


