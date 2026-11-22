---
title: "XmlSaveOptions.SheetIndexes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlSaveOptions. تمثل فهارس الأوراق المُصدَّرة"
type: docs
url: /ar/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

يمثل فهارس الأوراق المصدرة.

```csharp
public int[] SheetIndexes { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // ملء بعض البيانات في جميع الأوراق
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // إنشاء نسخة من XmlSaveOptions
            XmlSaveOptions options = new XmlSaveOptions();

            // في البداية تصدير جميع الأوراق (SheetIndexes فارغ)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // تعيين لتصدير الورقة الأولى والثالثة فقط (الفهارس 0 و 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // حفظ باستخدام الأوراق المحددة فقط
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // تغيير لتصدير الورقة الثانية فقط (الفهرس 1)
            options.SheetIndexes = new int[] { 1 };

            // حفظ باختيار أوراق مختلف
            workbook.Save("XmlExportSingleSheet.xml", options);

            // تعيين SheetIndexes إلى فارغ لتصدير جميع الأوراق
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### انظر أيضًا

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


