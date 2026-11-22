---
title: "الفئة SignatureLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.SignatureLine. تمثل خط التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

يمثل خط التوقيع.

```csharp
public class SignatureLine
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SignatureLine](signatureline/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | يشير إلى ما إذا كان يمكن إرفاق التعليقات. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | يحصل أو يعيّن البريد الإلكتروني للمغني. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | يحصل أو يعيّن المعرف لهذا خط التوقيع. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | يحصل أو يعيّن النص المعروض للمستخدم عند توقيع. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | يشير إلى ما إذا كان خط توقيع. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | يحصل أو يعيّن معرف موفر التوقيع. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | يشير إلى ما إذا كان يُظهر تاريخ التوقيع. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | يحصل أو يعيّن نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى {0000000000-0000-0000-0000-0000000000}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً {000CD6A4-0000-0000-C000-000000000046}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى تعيينها من قبل المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | يحصل أو يعيّن الموقع. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | يحصل أو يعيّن لقب المغني. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة صورة
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // إنشاء كائن سطر التوقيع
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // عيّن كائن خط التوقيع إلى الخاصية Picture.SignatureLine
            pic.SignatureLine = s;

            // احفظ ملف Excel
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


