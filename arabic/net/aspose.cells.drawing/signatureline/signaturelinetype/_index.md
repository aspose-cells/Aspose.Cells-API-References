---
title: "SignatureLine.SignatureLineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. تحصل أو تعين نوع التوقيع. Default  عندما يتم تعيين القيمة الافتراضية تكون قيمة ProviderId المقابلة ثابتة على 00000000000000000000000000000000. Stamp  عندما تكون القيمة Stamp تكون قيمة ProviderId المقابلة عادةً 000CD6A400000000C000000000000046. Custom  عندما تكون القيمة Custom عادةً يحتاج المستخدم إلى تعيين قيمة ProviderId المقابلة. يجب الحصول عليها من الوثائق المرفقة مع الموفر"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

يحصل أو يعيّن نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى {0000000000-0000-0000-0000-0000000000}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً {000CD6A4-0000-0000-C000-000000000046}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى تعيينها من قبل المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء سطر توقيع
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // عرض SignatureLineType الحالي
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // تعيين SignatureLineType إلى Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // إضافة سطر التوقيع إلى ورقة العمل عن طريق إضافته إلى الأشكال
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // تغيير SignatureLineType إلى Custom مع ProviderId مخصص
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // احفظ المصنف
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


