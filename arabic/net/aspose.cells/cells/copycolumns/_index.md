---
title: "Cells.CopyColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنسخ البيانات والتنسيقات لعمود كامل"
type: docs
url: /ar/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

ينسخ البيانات والتنسيقات لعمود كامل.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | Int32 | مؤشر العمود المصدر. |
| destinationColumnIndex | Int32 | مؤشر العمود الوجهة. |
| columnNumber | Int32 | رقم العمود المنسوخ. |
| pasteOptions | PasteOptions | خيارات اللصق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // إنشاء مصنف آخر كوجهة
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // نسخ الأعمدة مع التنسيق فقط
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // احفظ المصنف
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

ينسخ البيانات والتنسيقات لأعمدة كاملة.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | Int32 | مؤشر العمود المصدر. |
| destinationColumnIndex | Int32 | مؤشر العمود الوجهة. |
| columnNumber | Int32 | رقم العمود المنسوخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إضافة بيانات نموذجية إلى الأعمدة
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // نسخ الأعمدة من الفهرس 1 (B) إلى الفهرس 3 (D)، نسخ عمود واحد
            cells.CopyColumns(cells, 1, 3, 1);

            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

ينسخ البيانات والتنسيقات للأعمدة الكاملة.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | Int32 | مؤشر العمود المصدر. |
| sourceTotalColumns | Int32 | عدد الأعمدة المصدر. |
| destinationColumnIndex | Int32 | مؤشر العمود الوجهة. |
| destinationTotalColumns | Int32 | عدد الأعمدة الوجهة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ملء الأعمدة المصدر (الأعمدة 0 و 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // نسخ عمودين من الفهرس 0 إلى الفهرس الوجهة 3، وإدراج عمودين
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // التحقق من النسخ عن طريق فحص الأعمدة الوجهة (3 و 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


