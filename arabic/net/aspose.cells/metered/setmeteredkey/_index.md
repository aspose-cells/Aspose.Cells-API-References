---
title: "Metered.SetMeteredKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Metered. تعيين المفتاح العام والخاص للـ metered. إذا قمت بشراء ترخيص metered عند بدء التطبيق يجب استدعاء هذه API عادةً وهذا يكفي. ومع ذلك إذا فشل دائمًا في رفع بيانات الاستهلاك وتجاوز 24 ساعة سيتم ضبط الترخيص إلى حالة التقييم لتجنب هذه الحالة يجب عليك فحص حالة الترخيص بانتظام إذا كانت حالة التقييم استدعِ هذه API مرة أخرى."
type: docs
url: /ar/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

يضبط المفتاح العام والخاص للقياس. إذا قمت بشراء ترخيص مقاس، عند بدء التطبيق، يجب استدعاء هذه الواجهة البرمجية (API)، عادةً يكون ذلك كافيًا. ومع ذلك، إذا فشل دائمًا تحميل بيانات الاستهلاك وتجاوز 24 ساعة، سيتم تعيين الترخيص إلى حالة التقييم؛ لتجنب هذه الحالة، يجب عليك فحص حالة الترخيص بانتظام، إذا كانت في حالة التقييم، استدعِ هذه الواجهة البرمجية مرة أخرى.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| publicKey | String | المفتاح العام |
| privateKey | String | المفتاح الخاص |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // تعيين المفاتيح العامة والخاصة المقاسة
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // الحصول على كمية الاستهلاك المقاسة
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // الحصول على رصيد الاستهلاك المقاس
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


