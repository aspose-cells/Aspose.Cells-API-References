---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ OdsLoadOptions. يمثل خيارات تحميل ملف ods"
type: docs
url: /ar/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

يمثل خيارات تحميل ملف ods.

```csharp
public OdsLoadOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء OdsLoadOptions باستخدام المُنشئ
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // تعيين نمط الارتباط التشعبي لاستخدام الإعدادات الافتراضية لـ Excel
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // تحميل ملف ODS باستخدام خيارات التحميل
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // حفظ كـ XLSX
            workbook.Save("output.xlsx");
            
            // تحقق من تطبيق نمط الارتباط التشعبي
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### انظر أيضًا

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

يمثل خيارات تحميل ملف ods.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | LoadFormat | نوع تنسيق التحميل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // إنشاء ملف ODS تجريبي إذا لم يكن موجودًا
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // إنشاء OdsLoadOptions مع معامل LoadFormat
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // تحميل دفتر العمل باستخدام خيارات التحميل التي تم إنشاؤها
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // حفظ لتوضيح التحميل الناجح
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


