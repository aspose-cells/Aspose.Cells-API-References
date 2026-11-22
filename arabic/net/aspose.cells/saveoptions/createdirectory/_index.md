---
title: "SaveOptions.CreateDirectory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. إذا كانت true ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف"
type: docs
url: /ar/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

```csharp
public bool CreateDirectory { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // تعيين خيارات الحفظ مع تمكين CreateDirectory
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // حفظ المصنف في دليل جديد (سيتم إنشاؤه تلقائيًا)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


