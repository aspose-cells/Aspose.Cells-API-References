---
title: "PageSetup.Order"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة"
type: docs
url: /ar/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة.

```csharp
public PrintOrderType Order { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين ترتيب الطباعة إلى DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // احفظ دفتر العمل بصيغ مختلفة
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // غيّر ترتيب الطباعة إلى OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // احفظ مرة أخرى بصيغ مختلفة
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### انظر أيضًا

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


