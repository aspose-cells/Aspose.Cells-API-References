---
title: "Cells.InsertRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُدرج عدة صفوف في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

يدرج عدة صفوف في ورقة العمل.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |
| totalRows | Int32 | عدد الصفوف التي سيتم إدراجها. |
| updateReference | منطقي | يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // إدراج صف عند الفهرس 2 (سيصبح الصف الجديد هو الصف 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // إضافة بيانات إلى الصف المُدرج
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // احفظ المصنف
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

يدرج عدة صفوف في ورقة العمل.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |
| totalRows | Int32 | عدد الصفوف التي سيتم إدراجها. |
| خيارات | InsertOptions | خيارات عملية الإدراج. |

### أمثلة

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // إدراج 3 صفوف عند فهرس الصف 5 باستخدام الخيارات المحددة
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

يدرج عدة صفوف في ورقة العمل.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |
| totalRows | Int32 | عدد الصفوف التي سيتم إدراجها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بعض البيانات التجريبية
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // إدراج صفين عند فهرس الصف 2
            cells.InsertRows(2, 2);

            // تحقق من أن الصفوف المُدرجة فارغة
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // احفظ المصنف
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


