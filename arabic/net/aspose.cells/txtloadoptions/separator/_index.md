---
title: "TxtLoadOptions.Separator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. يحصل ويضبط فاصل الأحرف لملف النص"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

يحصل على ويضبط فاصل الأحرف لملف النص.

```csharp
public char Separator { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // إنشاء بيانات عينة وحفظها بفاصل مخصص
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // تحميل الملف المحفوظ بنفس الفاصل
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // تحقق من البيانات المحملة
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


