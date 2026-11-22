---
title: "Metered.GetProductName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Metered. يحصل على اسم المنتج"
type: docs
url: /ar/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

يحصل على اسم المنتج

```csharp
public string GetProductName()
```

### قيمة الإرجاع

اسم المنتج

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // إنشاء نسخة metered
            Metered metered = new Metered();
            
            // تعيين مفاتيح metered (استبدل بالمفاتيح الفعلية)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // احصل على اسم المنتج وعرضه
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // توضيح الاستخدام الأساسي مع جدول بيانات بسيط
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


