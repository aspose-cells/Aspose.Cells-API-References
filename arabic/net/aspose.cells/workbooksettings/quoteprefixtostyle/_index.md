---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان يتم تعيين خاصية QuotePrefix عند إدخال قيمة نصية تبدأ بعلامة اقتباس مفردة إلى الخلية"
type: docs
url: /ar/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

تشير إلى ما إذا كان يتم تعيين خاصية [`QuotePrefix`](../../style/quoteprefix/) عند إدخال قيمة نصية (تبدأ بعلامة اقتباس مفردة) إلى الخلية

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyQuotePrefixToStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // تمكين QuotePrefixToStyle - السلاسل التي تبدأ بـ' ستحصل على نمط QuotePrefix المطبق
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // تعطيل QuotePrefixToStyle - السلاسل تحتفظ بقيمتها الحرفية
            workbook.Settings.QuotePrefixToStyle = false;
            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.PutValue("'abc");
            Console.WriteLine("Cell A2 - QuotePrefix: " + cell2.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A2 - Value: " + cell2.StringValue);

            workbook.Save("QuotePrefixToStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


