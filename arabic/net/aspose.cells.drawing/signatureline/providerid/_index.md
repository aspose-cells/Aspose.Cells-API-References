---
title: "SignatureLine.ProviderId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. يحصل أو يضبط معرف موفر التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

يحصل أو يعيّن معرف موفر التوقيع.

```csharp
public Guid ProviderId { get; set; }
```

### ملاحظات

عادةً ما يكون CLSID لإضافة COM الخاصة بالموفر.

### أمثلة

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // إنشاء سطر توقيع جديد
            SignatureLine signatureLine = new SignatureLine();
            
            // تعيين خصائص سطر التوقيع
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // تعيين معرف الموفر (مثال GUID - يجب استبداله بمعرف GUID الفعلي للموفر)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // تعيين نوع التوقيع (يجب أن يتطابق مع معرف الموفر)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // إخراج معرف الموفر لإظهار الاستخدام
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


