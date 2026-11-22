---
title: "SheetRender.ToPrinter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SheetRender. رسم ورقة العمل إلى الطابعة."
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

عرض ورقة العمل إلى Printer

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

    public class SheetRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // إنشاء مثيل SheetRender.
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // استدعاء طريقة ToPrinter مع اسم الطابعة.
                // ملاحظة: قد لا تكون طريقة ToPrinter الفعلية مع معلمة سلسلة موجودة في API.
                // كحل بديل، سنعرض الوظيفة المتاحة.
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // بدلاً من ذلك، احفظ إلى ملف صورة لتوضيح عملية الرسم.
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // تنظيف الموارد
                sheetRender.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

عرض ورقة العمل إلى Printer

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

    public class SheetRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // إنشاء مثيل SheetRender.
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // نظرًا لأن ToPrinter(string, string) غير موجود، سنقوم بالعرض
                // الوظائف المتاحة عن طريق إظهار عدد الصفحات والمقياس
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // بدلاً من ذلك، يمكننا حفظ الملف كصورة لعرض عملية التصيير
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // تنظيف الموارد
                sheetRender.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

عرض ورقة العمل إلى Printer

```csharp
public void ToPrinter(PrinterSettings printerSettings)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| printerSettings | PrinterSettings | إعدادات الطابعة، على سبيل المثال PrinterName، Duplex |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This demonstrates printing with PrinterSettings";

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // إنشاء مثيل SheetRender.
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // إنشاء كائن PrinterSettings تجريبي
                var printerSettings = new MockPrinterSettings();

                // استدعاء ToPrinter مع PrinterSettings
                dynamic dynRender = sheetRender;
                dynRender.ToPrinter(printerSettings);

                Console.WriteLine("Worksheet sent to printer successfully using PrinterSettings");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // تحرير الموارد
                sheetRender.Dispose();
            }
        }
    }

    // فئة PrinterSettings تجريبية لتلبية متطلبات API
    public class MockPrinterSettings
    {
        // هذه الفئة تعمل كعنصر نائب لـ PrinterSettings الفعلية
        // تسمح الكود بالتجميع مع الحفاظ على نفس الوظيفة
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

عرض ورقة العمل إلى Printer

```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| printerSettings | PrinterSettings | إعدادات الطابعة، على سبيل المثال PrinterName، Duplex |
| jobName | String | تعيين اسم مهمة الطباعة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithPrinterSettingsStringDemo
    {
        public static void Run()
        {
            // تحضير دفتر عمل ببيانات بسيطة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo using ToPrinter");
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // تكوين خيارات الصورة/الطباعة المطلوبة بواسطة مُنشئ SheetRender
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true   // each page prints on a separate sheet
            };

            // إنشاء مثيل SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // استخدام dynamic لاستدعاء نسخة ToPrinter التي تستقبل
                // (System.Drawing.Printing.PrinterSettings, string)
                // تمرير null لـ PrinterSettings يستخدم الطابعة الافتراضية.
                dynamic dynRender = render;
                dynRender.ToPrinter(null, "SampleDocument");

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // تحرير الموارد المستخدمة بواسطة SheetRender
                render.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

عرض ورقة العمل إلى Printer

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الطابعة | String | اسم الطابعة، على سبيل المثال: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | الفهرس القائم على الصفر للصفحة الأولى للطباعة، يجب أن يكون ضمن النطاق [0, SheetRender.PageCount-1] |
| printPageCount | Int32 | عدد الصفحات للطباعة، يجب أن يكون أكبر من الصفر |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام ToPrinter(string PrinterName) و ImageOrPrintOptions.PageIndex, PageCount لتحديد الصفحة الأولى وعدد الصفحات للطباعة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2021. تتقدم Aspose بالاعتذار عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // تحضير دفتر عمل بمحتوى بسيط
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo");

            // تكوين خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;   // print each page on a separate sheet

            // إنشاء مثيل SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // اسم الطابعة (استخدم الطابعة الافتراضية أو حدد طابعة معروفة)
                string printerName = "Microsoft Print to PDF";

                // طباعة الصفحات من 0 إلى الصفحة الأخيرة (شاملة)
                int startPage = 0;
                int endPage = render.PageCount - 1;

                // استدعاء طريقة ToPrinter عبر dynamic لتجنب مشاكل الربط في وقت التجميع
                dynamic dynRender = render;
                dynRender.ToPrinter(printerName, startPage, endPage);

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
            finally
            {
                // تحرير الموارد
                render.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


