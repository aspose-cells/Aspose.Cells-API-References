---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlSaveOptions. تشير إلى ما إذا كان تصدير البيانات كسمات للعنصر"
type: docs
url: /ar/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

يشير إلى ما إذا كان يتم تصدير البيانات كسمات للعنصر.

```csharp
public bool DataAsAttribute { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // إنشاء خيارات حفظ XML مع تعيين DataAsAttribute إلى true
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // حفظ البيانات كسمات
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // تغيير لحفظ البيانات كعناصر
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


