---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DbfLoadOptions. الخيارات"
type: docs
url: /ar/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

الخيارات.

```csharp
public DbfLoadOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء كائن DbfLoadOptions باستخدام طريقة #ctor
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // إنشاء مصنف باستخدام خيارات تحميل DBF
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض بعض البيانات من ملف DBF المحمَّل
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // احفظ المصنف بتنسيق Excel
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


