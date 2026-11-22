---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. في ms excel عند نسخ صيغ تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل بنفس الاسم في نفس المصنف، مثل عندما تم نسخ تلك الأوراق مسبقًا قبل عملية النسخ هذه، يجب أن تُحافظ على هذه الخاصية كـ true."
type: docs
url: /ar/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل ذات الاسم نفسه في نفس المصنف، مثل عندما تكون تلك الأوراق قد تم نسخها قبل عملية النسخ هذه، لذا يجب الحفاظ على هذه الخاصية كقيمة true.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف قالب مع بيانات عينة
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // إنشاء مصنف الإخراج
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // نسخ أوراق العمل مع تمكين ReferToSheetWithSameName
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // تحقق من أن الصيغة تشير إلى الورقة الصحيحة
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


