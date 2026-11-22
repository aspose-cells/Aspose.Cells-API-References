---
title: "Worksheet.AutoFitRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تضبط تلقائيًا جميع الصفوف في هذه ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

يضبط جميع الصفوف في هذه ورقة العمل تلقائيًا.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | AutoFitterOptions | خيارات الضبط التلقائي |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات نموذجية وتنسيق
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // دمج الخلايا لتوضيح الضبط التلقائي للخلية المدمجة
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // ضبط تلقائي للصفوف بخيارات محددة
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // احفظ المصنف
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int) {#autofitrows_3}

يضبط ارتفاع الصف في نطاق تلقائيًا.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء الخلايا ببيانات نموذجية وأنماط
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // ضبط تلقائي للصفوف من الفهرس 0 إلى 8
            sheet.AutoFitRows(0, 8);

            // إخراج ارتفاعات الصفوف الناتجة
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

يضبط ارتفاع الصف في نطاق تلقائيًا.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| خيارات | AutoFitterOptions | خيارات الضبط التلقائي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // إنشاء خيارات الضبط التلقائي
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // ضبط تلقائي للصفوف من 0 إلى 1 مع الخيارات
            worksheet.AutoFitRows(0, 1, options);
            
            // احفظ المصنف
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows() {#autofitrows}

يضبط جميع الصفوف في هذه ورقة العمل تلقائيًا.

```csharp
public void AutoFitRows()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // ضبط تلقائي للصفوف
            worksheet.AutoFitRows();
            
            // ضبط تلقائي للأعمدة لتحسين الرؤية
            worksheet.AutoFitColumns();
            
            // احفظ المصنف
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

يضبط جميع الصفوف في هذه ورقة العمل تلقائيًا.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| onlyAuto | منطقي | True، يضبط تلقائيًا ارتفاع الصف فقط عندما لا يكون الارتفاع مخصصًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نص نموذجي إلى الخلايا لتوضيح الضبط التلقائي للصف
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // ضبط تلقائي للصفوف مع مراعاة الدمج التلقائي
            worksheet.AutoFitRows(true);
            
            // احفظ المصنف
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


