---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة الأولية كما يفعل ms excel. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

يشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة الأولية كما يفعل ms excel. القيمة الافتراضية هي true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### ملاحظات

نفس القاعدة في ms excel، لن يتم اعتبار الصف/العمود فارغًا إذا كان لديه نمط مخصص، حتى وإن لم يحتوي على بيانات خلية. عند الحفظ باستخدام وضع LightCells، لا يؤثر هذا الخيار. يجب على المستخدم التحكم في نطاق الإخراج من خلال تنفيذ [`LightCellsDataProvider`](../lightcellsdataprovider/) أو بتحديد [`ExportArea`](../exportarea/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي يحتوي على بعض البيانات وصفوف/أعمدة فارغة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات مع صفوف/أعمدة فارغة أولية
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // حفظ دون قص الفراغات الأولية
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // حفظ مع قص الفراغات الأولية
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


