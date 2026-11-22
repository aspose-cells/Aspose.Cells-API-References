---
title: "ExternalLink.AddExternalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ExternalLink. تضيف اسمًا خارجيًا"
type: docs
url: /ar/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

يضيف اسمًا خارجيًا.

```csharp
public void AddExternalName(string text, string referTo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص الاسم الخارجي. إذا كان الاسم الخارجي ينتمي إلى ورقة عمل، يجب أن يكون النص على الشكل Sheet1!Text. |
| referTo | String | الـ referTo للاسم الخارجي. يجب أن يكون خلية أو نطاقًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء مصنف خارجي تجريبي
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // أضف رابطًا خارجيًا إلى المصنف الرئيسي
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // أضف اسمًا خارجيًا
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // استخدم الاسم الخارجي في صيغة
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // احسب الصيغة
            workbook.CalculateFormula();
            
            // أخرج النتيجة.
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


