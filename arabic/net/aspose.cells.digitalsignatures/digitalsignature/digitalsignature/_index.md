---
title: "DigitalSignature.DigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DigitalSignature. مُنشئ digitalSignature. يستخدم تنفيذ .Net"
type: docs
url: /ar/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

منشئ digitalSignature. يستخدم تنفيذ .Net.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| شهادة | X509Certificate2 | كائن الشهادة الذي تم استخدامه لتوقيع المستند. |
| تعليقات | String | الغرض من التوقيع. |
| signTime | DateTime | وقت UTC عندما تم توقيع المستند. |

### أمثلة

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // إنشاء مجموعة توقيع رقمي
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // تحميل الشهادة مع المفتاح الخاص
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // إنشاء توقيع رقمي باستخدام الشهادة، الغرض والطابع الزمني
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // إنشاء دفتر عمل جديد وتوقيعه
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

منشئ digitalSignature. يستخدم تنفيذ Bouncy Castle.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rawData | Byte[] | مصفوفة بايت تحتوي على بيانات من شهادة X.509. |
| كلمة المرور | String | كلمة المرور المطلوبة للوصول إلى بيانات شهادة X.509. |
| تعليقات | String | الغرض من التوقيع. |
| signTime | DateTime | وقت UTC عندما تم توقيع المستند. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض المحتوى التجريبي
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // تحميل ملف الشهادة كمصفوفة بايت (استبدل بمسار الشهادة الفعلي)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // إنشاء معلمات التوقيع الرقمي
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // استدعاء المُنشئ مع (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // إنشاء DigitalSignatureCollection وإضافة التوقيع إليه
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // إضافة التوقيعات إلى دفتر العمل
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


