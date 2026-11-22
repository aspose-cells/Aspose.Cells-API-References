---
title: "PasteOptions.KeepOldTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. تحتفظ بالجداول في النطاق الوجهة"
type: docs
url: /ar/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

يحافظ على الجداول في النطاق الوجهة.

```csharp
public bool KeepOldTables { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية مع البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // إنشاء مثيل PasteOptions
                PasteOptions pasteOptions = new PasteOptions();

                // عرض القيمة الافتراضية لخاصية KeepOldTables
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // تعيين KeepOldTables إلى true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // إنشاء نطاقات لعملية النسخ
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // نسخ مع خيار KeepOldTables
                targetRange.Copy(sourceRange, pasteOptions);

                // احفظ المصنف
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


