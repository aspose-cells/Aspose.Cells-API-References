---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlSaveOptions. تشير إلى ما إذا كان يتم تصدير اسم الورقة كاسم العنصر"
type: docs
url: /ar/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

يشير إلى ما إذا كان يتم تصدير اسم الورقة كاسم للعنصر.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي يحتوي على بيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // حفظ مع SheetNameAsElementName = true (الافتراضي)
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // حفظ مع SheetNameAsElementName = false
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### انظر أيضًا

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


