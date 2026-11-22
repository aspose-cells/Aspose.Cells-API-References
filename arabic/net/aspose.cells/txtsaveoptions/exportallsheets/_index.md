---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. إذا كانت false فسيتم تصدير الورقة النشطة فقط كما في MS Excel"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

يشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. إذا كان خاطئًا، يتم تصدير الورقة النشطة فقط، مثل MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف بورقتين
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // إضافة بيانات نموذجية إلى كلتا الورقتين
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // حفظ مع ExportAllSheets=false (الافتراضي)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // حفظ مع ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


