---
title: "XmlLoadOptions.ContainsMultipleWorksheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تشير إلى ما إذا كان استيراد xml كأوراق عمل متعددة"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

يشير إلى ما إذا كان استيراد XML كأوراق عمل متعددة.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // إنشاء ملف Excel تجريبي يحتوي على أوراق عمل متعددة
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
            workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // حفظ كـ XML مع أوراق عمل متعددة
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output.xml", saveOptions);

            // تحميل XML مع ContainsMultipleWorksheets=true
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);

            // تحقق من تحميل كلتا ورقتي العمل
            Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
            Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
            Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


