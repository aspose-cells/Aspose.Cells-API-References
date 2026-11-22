---
title: "LoadOptions.LoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ LoadOptions. ينشئ خيارات لتحميل الملف"
type: docs
url: /ar/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

إنشاء خيارات تحميل الملف.

```csharp
public LoadOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // إنشاء محتوى CSV نموذجي
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // إظهار المنشئ الافتراضي
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // إظهار المنشئ مع معامل LoadFormat
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // تحميل ملف CSV مع الخيارات المحددة
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // التحقق من تحميل البيانات بشكل صحيح
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // احفظ كملف XLSX لتوضيح التحويل
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

إنشاء خيارات تحميل الملف.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | LoadFormat | صيغة التحميل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // إنشاء محتوى CSV نموذجي
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // إنشاء LoadOptions مع LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // تحميل ملف CSV باستخدام الخيارات التي تم إنشاؤها
                Workbook workbook = new Workbook(tempCsvPath, options);

                // إظهار التحميل الناجح عن طريق قراءة الخلية
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // احفظ كملف XLSX لإظهار قدرة التحويل
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


