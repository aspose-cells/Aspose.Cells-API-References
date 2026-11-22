---
title: "Style.CultureCustom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل وتعيّن سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن فسيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا فستُرجع سلسلة النمط المقابلة للرقم المدمج"
type: docs
url: /ar/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

يحصل على سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام ويضبطها. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج.

```csharp
public string CultureCustom { get; set; }
```

### ملاحظات

بالنسبة لتنسيق الأرقام المدمج، كل من محتوى النمط (مثلًا، أحد تنسيقات التاريخ المدمجة هو "m/d/y" لبعض المناطق، ولكن لبعض المناطق الأخرى يصبح "d/m/y") ومحدد التنسيق (مثلًا، بعض المناطق تستخدم حرفًا غير 'y' لتمثيل جزء السنة في تنسيق التاريخ) يعتمد على الثقافة؛ بالنسبة للتنسيق المخصص المحدد من قبل المستخدم، يتم تغيير محددات التنسيق فقط وفقًا للثقافة، بينما لا يتم تعديل الأجزاء الأخرى من نمط التنسيق.

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا واضبط الثقافة الهنغارية
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // احصل على الخلية الأولى ونمطها
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // عيّن تنسيقًا مخصصًا وأظهر تحويل CultureCustom
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // طبق النمط وأظهر التنسيق المتوافق مع الثقافة
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // أظهر الصيغة مع تنسيق الثقافة
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


