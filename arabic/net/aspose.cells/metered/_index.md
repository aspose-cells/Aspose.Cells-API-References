---
title: "الفئة Metered"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Metered. توفر طرقًا لتعيين مفتاح القياس"
type: docs
url: /ar/net/aspose.cells/metered/
---
## Metered class

يوفر طرقًا لتعيين المفتاح القابل للقياس.

```csharp
public class Metered
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Metered](metered/)() | يُنشئ مثيلًا جديدًا لهذه الفئة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | يحصل على اسم المنتج |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | يضبط المفتاح العام والخاص للقياس. إذا قمت بشراء ترخيص مقاس، عند بدء التطبيق، يجب استدعاء هذه الواجهة البرمجية (API)، عادةً يكون ذلك كافيًا. ومع ذلك، إذا فشل دائمًا تحميل بيانات الاستهلاك وتجاوز 24 ساعة، سيتم تعيين الترخيص إلى حالة التقييم؛ لتجنب هذه الحالة، يجب عليك فحص حالة الترخيص بانتظام، إذا كانت في حالة التقييم، استدعِ هذه الواجهة البرمجية مرة أخرى. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | يحصل على رصيد الاستهلاك |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | يحصل على حجم ملف الاستهلاك |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | تحقق مما إذا كان Metered مرخصًا |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // إنشاء مثيل من الفئة Metered
            Metered metered = new Metered();

            // تعيين مفتاح Metered
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // احصل على اسم المنتج واعرضه
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // كود إضافي لتوضيح كيفية استخدام المثيل
            // على سبيل المثال، إنشاء مصنف وحفظه
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


