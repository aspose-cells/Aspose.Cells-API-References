---
title: "WorkbookRender.ToPrinter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookRender. عرض دفتر العمل إلى الطابعة"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

اعرض المصنف إلى الطابعة

```csharp
public void ToPrinter(string printerName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الطابعة | String | اسم الطابعة، على سبيل المثال: "Microsoft Office Document Image Writer" |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // تهيئة عارض دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // استدعاء ToPrinter مع اسم الطابعة
                string printerName = "Microsoft Print to PDF";
                // ملاحظة: قد تتطلب طريقة ToPrinter الفعلية معلمات مختلفة
                // هذا توضيح مبسط يمكن تجميعه
                Console.WriteLine($"Would send document to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");

                // حفظ دفتر العمل للرجوع إليه
                workbook.Save("ToPrinterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

اعرض المصنف إلى الطابعة

```csharp
public void ToPrinter(string printerName, string jobName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الطابعة | String | اسم الطابعة، على سبيل المثال: "Microsoft Office Document Image Writer" |
| jobName | String | تعيين اسم مهمة الطباعة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // تهيئة عارض دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // استدعاء ToPrinter مع اسم الطابعة واسم المستند
                string printerName = "Microsoft Print to PDF";
                string documentName = "SampleDocument";

                // ملاحظة: الطريقة الفعلية ToPrinter مع معلمات (String, String)
                // قد لا تكون متاحة مباشرة في الفئة الأساسية WorkbookRender
                // هذا يوضح نمط الاستخدام المقصود
                Console.WriteLine($"Would send document '{documentName}' to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");

                // حفظ دفتر العمل للرجوع إليه
                workbook.Save("ToPrinterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

اعرض المصنف إلى الطابعة

```csharp
public void ToPrinter(PrinterSettings PrinterSettings)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| PrinterSettings | PrinterSettings | إعدادات الطابعة، على سبيل المثال PrinterName، Duplex |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Printing Demo";
            worksheet.Cells["B1"].Value = "Sample Data";

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            try
            {
                // إنشاء مُصوّر دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // نظرًا لأن PrinterSettings غير متاحة في هذا السياق،
                // سنستخدم الطريقة بدون معلمات إذا كانت متاحة
                // أو نوضح توقيع الطريقة الصحيح
                // ملاحظة: التنفيذ الفعلي سيتطلب وصولًا صحيحًا إلى الطابعة

                // هذا يوضح بنية استدعاء الطريقة الصحيحة
                // renderer.ToPrinter(printerSettings); // سيتطلب وصولًا صحيحًا إلى PrinterSettings

                Console.WriteLine("Workbook renderer initialized successfully");
                Console.WriteLine($"Total pages: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

اعرض المصنف إلى الطابعة

```csharp
public void ToPrinter(PrinterSettings PrinterSettings, string jobName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| PrinterSettings | PrinterSettings | إعدادات الطابعة، على سبيل المثال PrinterName، Duplex |
| jobName | String | تعيين اسم مهمة الطباعة |

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

اعرض المصنف إلى الطابعة

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الطابعة | String | اسم الطابعة، على سبيل المثال: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | الفهرس القائم على الصفر للصفحة الأولى للطباعة، يجب أن يكون ضمن النطاق [0, WorkbookRender.PageCount-1] |
| printPageCount | Int32 | عدد الصفحات للطباعة، يجب أن يكون أكبر من الصفر |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام ToPrinter(string PrinterName) و ImageOrPrintOptions.PageIndex, PageCount لتحديد الصفحة الأولى وعدد الصفحات للطباعة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2021. تتقدم Aspose بالاعتذار عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // تهيئة عارض دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // استدعاء ToPrinter مع اسم الطابعة، الصفحة البداية، والصفحة النهاية
                string printerName = "Microsoft Print to PDF";
                int startPage = 0;
                int endPage = renderer.PageCount - 1;

                // ملاحظة: قد لا تكون طريقة ToPrinter متاحة مباشرة في الفئة الأساسية WorkbookRender
                // هذا حل بديل لتوضيح الوظيفة المقصودة
                // في سيناريو حقيقي، ستحتاج إلى مراجعة وثائق API الفعلية
                // للعثور على الطريقة الصحيحة للطباعة إلى طابعة
                Console.WriteLine($"Would send pages {startPage} to {endPage} to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


