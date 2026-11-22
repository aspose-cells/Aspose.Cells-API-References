---
title: "XmlSaveOptions.HasHeaderRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlSaveOptions. تشير إلى ما إذا كان النطاق يحتوي على صف رأس"
type: docs
url: /ar/net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

يشير إلى ما إذا كان النطاق يحتوي على صف رأس.

```csharp
public bool HasHeaderRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة صف رأس والبيانات
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء خيارات حفظ XML
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
            saveOptions.SheetNameAsElementName = true;

            // حفظ كملف XML
            workbook.Save("output.xml", saveOptions);

            Console.WriteLine("XML file saved with HasHeaderRow=true");
        }
    }
}
```

### انظر أيضًا

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


