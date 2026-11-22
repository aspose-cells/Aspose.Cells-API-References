---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ TxtLoadOptions. ينشئ الخيارات لتحميل ملف النص"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

ينشئ الخيارات لتحميل ملف نصي.

```csharp
public TxtLoadOptions()
```

### ملاحظات

نوع ملف التحميل الافتراضي هو CSV.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء TxtLoadOptions جديد باستخدام المنشئ
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // تعيين الفاصل لملف CSV
            loadOptions.Separator = ',';
            
            // إنشاء دفتر عمل مع خيارات التحميل
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // إخراج بعض المعلومات من الملف المحمل
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

ينشئ الخيارات لتحميل ملف نصي.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | LoadFormat | تنسيق التحميل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // إنشاء محتوى CSV عينة وملف مؤقت
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // إنشاء TxtLoadOptions مع LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // تحميل CSV باستخدام الخيارات المكوّنة
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض البيانات المحملة
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // حفظ دفتر العمل المعالج
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // تنظيف الملف المؤقت
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


