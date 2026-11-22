---
title: "Style.SetCustom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تعيين سلسلة تنسيق الرقم المخصص لخلية"
type: docs
url: /ar/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

يضبط سلسلة تنسيق الرقم المخصص لخلية.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مخصص | String | سلسلة تنسيق الرقم المخصص، يجب أن تكون بنمط InvariantCulture. |
| builtinPreference | منطقي | إذا كانت سلسلة تنسيق الرقم المخصص المعطاة تطابق أحد تنسيقات الأرقام المدمجة المقابلة لإعدادات المنطقة الحالية، فهل يتم تعيين تنسيق الرقم كمدمج بدلاً من مخصص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


