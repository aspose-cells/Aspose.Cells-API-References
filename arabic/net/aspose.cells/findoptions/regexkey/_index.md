---
title: "FindOptions.RegexKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. تشير إلى ما إذا كان المفتاح الذي تم البحث عنه هو تعبير نمطي (regex). إذا كانت true سيتم اعتبار المفتاح تعبيرًا نمطيًا وتحليلَه. وإلا سيتم تحليل المفتاح وفقًا للقواعد في MS Excel"
type: docs
url: /ar/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

يشير إلى ما إذا كان المفتاح الذي تم البحث عنه هو تعبير نمطي. إذا كان صحيحًا سيتم اعتبار المفتاح كتعريف نمطي وتحليلّه. وإلا سيتم تحليل المفتاح وفقًا للقواعد في MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### ملاحظات

على الرغم من أنه تم تحديد مفتاح البحث كتعريف نمطي (regex)، قد يتم إعادة تشكيله وفقًا للـ[`LookAtType`](../lookattype/). على سبيل المثال، عندما يكون النوع هو Contains (هذا هو القيمة الافتراضية لهذه الخيارات)، ستُضاف أحرف البدل في بداية ونهاية مفتاح البحث تلقائيًا لضمان فحص المطابقة كـ "contains". في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وستنخفض الأداء أيضًا. لذلك، من منظور الأداء، إذا كان المستخدم قد حدد القاعدة الدقيقة للتعبير النمطي، فلا حاجة لاستخدام [`LookAtType`](../lookattype/) كقيد إضافي ويمكن للمستخدم تعيينه كـ EntireContent للحصول على أداء أفضل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // حدد بيانات اختبار بسلاسل مطابقة للنمط
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // أنشئ خيارات البحث مع تمكين regex
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // ابحث عن خلايا تطابق نمط regex
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // أخرج النتيجة.
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


