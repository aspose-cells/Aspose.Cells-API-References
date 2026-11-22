---
title: "Workbook.Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ Workbook. يهيئ نسخة جديدة من فئة Workbook"
type: docs
url: /ar/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

يهيئ نسخة جديدة من فئة [`Workbook`](../).

```csharp
public Workbook()
```

### ملاحظات

نوع تنسيق الملف الافتراضي هو Xlsx. إذا كنت تريد إنشاء أنواع أخرى من الملفات، يرجى استخدام Workbook(FileFormatType).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد باستخدام المنشئ
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // احفظ المصنف
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

يهيئ نسخة جديدة من فئة [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileFormatType | FileFormatType | تنسيق الملف الجديد. |

### ملاحظات

نوع تنسيق الملف الافتراضي هو Excel97To2003.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بتنسيق ملف XLSX
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضع بعض البيانات في الخلية A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

يُهيئ نسخة جديدة فارغة من الفئة [`Workbook`](../) مع الخيارات

```csharp
public Workbook(LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LoadOptions | الخيارات. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

يُهيئ نسخة جديدة من الفئة [`Workbook`](../) ويفتح ملفًا.

```csharp
public Workbook(string file)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | String | اسم الملف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // المسار إلى دليل المستندات.
            string dataDir = "Your Document Directory";

            // إنشاء مصنف من ملف Excel موجود
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض بعض معلومات ورقة العمل
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // حفظ المصنف بتنسيق MHTML
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // إنشاء مصنف آخر من ملف MHTML المحفوظ
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

يُهيئ نسخة جديدة من الفئة [`Workbook`](../) ويفتح تدفقًا.

```csharp
public Workbook(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | التدفق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // إنشاء ملف Excel تجريبي في الذاكرة
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // إنشاء نسخة جديدة من المصنف باستخدام مُنشئ Stream
                Workbook workbook = new Workbook(sampleStream);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض البيانات المحملة
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // حفظ المصنف إلى ملف
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

يُهيئ نسخة جديدة من الفئة [`Workbook`](../) ويفتح ملفًا.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | String | اسم الملف. |
| loadOptions | LoadOptions | خيارات التحميل |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل بدون LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // تهيئة المصنف بمسار الملف وخيارات التحميل
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // إظهار أن المصنف تم تحميله عبر الوصول إلى عدد أوراق العمل
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

يُهيئ نسخة جديدة من الفئة [`Workbook`](../) ويفتح تدفقًا.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | التدفق. |
| loadOptions | LoadOptions | خيارات التحميل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء ملف Excel تجريبي في الذاكرة
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // إنشاء LoadOptions بإعدادات محددة
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // إنشاء نسخة من المصنف باستخدام #ctor مع Stream وLoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // عرض معلومات أساسية حول المصنف المحمَّل
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // اعرض بعض محتوى الخلية إذا كان متاحًا
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // أنشئ ملف Excel بسيط في الذاكرة للتوضيح
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


