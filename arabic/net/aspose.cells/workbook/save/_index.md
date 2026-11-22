---
title: "Workbook.Save"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحفظ دفتر العمل على القرص"
type: docs
url: /ar/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

يحفظ المصنف على القرص.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم الملف. |
| saveFormat | SaveFormat | نوع تنسيق الحفظ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى الورقة الأولى وإضافة بعض البيانات التجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // حفظ دفتر العمل بتنسيق XLSX
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // حفظ دفتر العمل بتنسيق PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

احفظ المصنف على القرص.

```csharp
public void Save(string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // حفظ دفتر العمل بتنسيقات مختلفة باستخدام معلمة سلسلة
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

يحفظ المصنف على القرص.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم الملف. |
| saveOptions | SaveOptions | خيارات الحفظ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى الورقة الأولى وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // إنشاء خيارات حفظ HTML وتكوينها
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // حفظ دفتر العمل مع الخيارات
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

يحفظ المصنف إلى التدفق.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الملف. |
| saveFormat | SaveFormat | نوع تنسيق ملف الحفظ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى الورقة الأولى وإضافة بعض البيانات التجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // إنشاء دفق الذاكرة لحفظ دفتر العمل
                using (MemoryStream stream = new MemoryStream())
                {
                    // حفظ دفتر العمل إلى الدفق بتنسيق XLSX
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // عرض رسالة النجاح
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // إعادة تعيين موضع الدفق للمعالجة الإضافية المحتملة
                    stream.Position = 0;

                    // حفظ إلى ملف اختياريًا للتحقق
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

يحفظ المصنف إلى التدفق.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الملف. |
| saveOptions | SaveOptions | خيارات الحفظ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى الورقة الأولى وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // إنشاء MemoryStream لحفظ دفتر العمل
            MemoryStream stream = new MemoryStream();

            try
            {
                // إنشاء SaveOptions لتنسيق PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // حفظ دفتر العمل إلى الدفق مع الخيارات المحددة
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // إعادة تعيين موضع الدفق للاستخدام المحتمل لاحقًا
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // تنظيف الموارد
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

ينشئ ورقة النتائج وينقلها إلى العميل ثم يفتحها في المتصفح أو MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استجابة | HttpResponse | كائن الاستجابة لإرجاع جدول البيانات إلى العميل. |
| fileName | String | اسم الملف الذي تم إنشاؤه. |
| contentDisposition | ContentDisposition | نوع توزيع المحتوى. |
| saveOptions | SaveOptions | خيارات الحفظ. |

### ملاحظات

هذه الطريقة متاحة لإصدارات net4.x فقط.

### انظر أيضًا

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

ينشئ ورقة النتائج وينقلها إلى العميل ثم يفتحها في المتصفح أو MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| استجابة | HttpResponse | كائن الاستجابة لإرجاع جدول البيانات إلى العميل. |
| fileName | String | اسم الملف الذي تم إنشاؤه. |
| contentDisposition | ContentDisposition | نوع توزيع المحتوى. |
| saveOptions | SaveOptions | خيارات الحفظ. |
| enableHttpCompression | منطقي | ما إذا كان يجب استخدام ضغط http |

### ملاحظات

هذه الطريقة متاحة لإصدارات net4.x فقط.

### انظر أيضًا

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


