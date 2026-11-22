---
title: "Cells.CopyRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنسخ البيانات والتنسيقات لبعض الصفوف الكاملة"
type: docs
url: /ar/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | Int32 | فهرس الصف المصدر. |
| destinationRowIndex | Int32 | فهرس الصف الوجهة. |
| rowNumber | Int32 | رقم الصف المنسوخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // أضف بعض البيانات النموذجية إلى مصنف المصدر
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // احصل على الخلايا من كلا المصنفين
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // انسخ جميع الصفوف من المصدر إلى الوجهة بدءًا من الصف 0 في الوجهة
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // حفظ النتيجة
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | Int32 | فهرس الصف المصدر. |
| destinationRowIndex | Int32 | فهرس الصف الوجهة. |
| rowNumber | Int32 | رقم الصف المنسوخ. |
| copyOptions | CopyOptions | خيارات النسخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية والروابط التشعبية
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // أدرج صفًا فارغًا عند الصف 5
            worksheet.Cells.InsertRows(5, 1);

            // نسخ الصف 4 إلى الصف 5 بدون CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // إعادة تعيين ورقة العمل
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // إدراج صف فارغ عند الصف 5 مرة أخرى
            worksheet.Cells.InsertRows(5, 1);

            // نسخ الصف 4 إلى الصف 5 باستخدام CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells0 | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | Int32 | فهرس الصف المصدر. |
| destinationRowIndex | Int32 | فهرس الصف الوجهة. |
| rowNumber | Int32 | رقم الصف المنسوخ. |
| copyOptions | CopyOptions | خيارات النسخ. |
| pasteOptions | PasteOptions | خيارات اللصق. |

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


