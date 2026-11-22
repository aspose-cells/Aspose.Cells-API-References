---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DbfSaveOptions. خيارات حفظ ملف .dbf"
type: docs
url: /ar/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

خيارات حفظ ملف .dbf.

```csharp
public DbfSaveOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // إنشاء مثيل DbfSaveOptions باستخدام المنشئ
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // تعيين خصائص خيارات الحفظ
                saveOptions.ExportAsString = true;
                
                // حفظ المصنف باستخدام خيارات حفظ DBF
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


