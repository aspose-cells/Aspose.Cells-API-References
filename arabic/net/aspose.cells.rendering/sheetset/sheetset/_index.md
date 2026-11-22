---
title: "SheetSet.SheetSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ SheetSet. ينشئ مجموعة أوراق بناءً على فهارس الأوراق الدقيقة"
type: docs
url: /ar/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

ينشئ مجموعة أوراق بناءً على فهارس الأوراق الدقيقة.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndexes | Int32[] | فهارس الأوراق تبدأ من الصفر. |

### ملاحظات

إذا تم العثور على ورقة غير موجودة في دفتر العمل، سيتم رمي استثناء أثناء عملية التصيير.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على 3 أوراق عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // إضافة نص تعريف إلى كل ورقة
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // إنشاء SheetSet بفهارس أوراق محددة (0 و 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // إنشاء خيارات حفظ PDF باستخدام مجموعة الأوراق الخاصة بنا
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // حفظ دفتر العمل بالأوراق المحددة
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

ينشئ مجموعة أوراق بناءً على أسماء الأوراق الدقيقة.

```csharp
public SheetSet(params string[] sheetNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetNames | String[] | أسماء الأوراق. |

### ملاحظات

إذا تم العثور على ورقة غير موجودة في دفتر العمل، سيتم رمي استثناء أثناء عملية التصيير.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد وإضافة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // تحضير أسماء الأوراق لـ SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // إنشاء SheetSet باستخدام معامل مصفوفة نصية
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // تكوين خيارات حفظ PDF باستخدام SheetSet المُنشأ
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // حفظ دفتر العمل كملف PDF مع الأوراق المحددة
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


