---
title: "Style.InvariantCustom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل على سلسلة النمط المستقلة عن الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج"
type: docs
url: /ar/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

يحصل على سلسلة النمط المستقلة عن الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج.

```csharp
public string InvariantCustom { get; }
```

### ملاحظات

بالنسبة لتنسيقات الأرقام المدمجة، لا يزال محتوى النمط المرتجع يعتمد على الثقافة، مثلًا، لبعض المناطق يُعيد "m/d/y" وللبعض الآخر يُعيد "d/m/y". الفرق عن [`CultureCustom`](../culturecustom/) هو (وهذا أيضًا ما يعنيه الاستقلال عن الثقافة): يتم الحفاظ على محددات التنسيق والفواصل كمعايير، مثل أن '/' سيُستخدم دائمًا كفاصل للوقت والتاريخ و"y" سيُستخدم دائمًا كجزء "السنة" بغض النظر عن أي حرف خاص آخر يُستخدم للمنطقة المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // تعيين تنسيق التاريخ والقيمة
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // إخراج النتائج
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


