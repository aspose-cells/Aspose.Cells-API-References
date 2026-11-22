---
title: "LoadOptions.LoadFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل على تنسيق التحميل"
type: docs
url: /ar/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

يحصل على تنسيق التحميل.

```csharp
public LoadFormat LoadFormat { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // إنشاء ملف CSV تجريبي
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // إنشاء LoadOptions لتنسيق CSV وعرض الخاصية
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // تحميل CSV باستخدام الخيارات الصحيحة
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // إنشاء LoadOptions لتنسيق XLSX وعرض الخاصية
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // إنشاء/حفظ ملف XLSX تجريبي
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // تحميل XLSX باستخدام الخيارات الصحيحة
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // تنظيف الملفات المؤقتة
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


