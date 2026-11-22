---
title: "InsertOptions.CopyFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية InsertOptions."
type: docs
url: /ar/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // اضبط القيم والتنسيق للعرض
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // إنشاء InsertOptions وتعيين CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // أدرج صفًا بالتنسيق من الأعلى
            worksheet.Cells.InsertRows(2, 1, options);

            // حفظ النتيجة
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


