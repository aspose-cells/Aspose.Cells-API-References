---
title: "DataSorter.Sort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DataSorter. تقوم بفرز بيانات المنطقة"
type: docs
url: /ar/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

يرتب بيانات المنطقة.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الخلايا | الخلايا | الخلايا تحتوي على منطقة البيانات. |
| startRow | Int32 | صف البداية للمنطقة. |
| startColumn | Int32 | عمود البداية للمنطقة. |
| endRow | Int32 | صف النهاية للمنطقة. |
| endColumn | Int32 | عمود النهاية للمنطقة. |

### قيمة الإرجاع

المؤشرات الأصلية (الموضع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى التحريك بواسطة عملية الفرز هذه، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // ملء بيانات عينة
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // إخفاء صف لإظهار الفرز مع الصفوف المخفية
            cells.Rows[1].IsHidden = true;
            
            // إنشاء وتكوين المُرتّب
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // إظهار طريقة Sort مع Cells ومعلمات Int32
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // إخراج النتائج إلى وحدة التحكم
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

رتّب بيانات المنطقة.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الخلايا | الخلايا | الخلايا تحتوي على منطقة البيانات. |
| منطقة | CellArea | المنطقة المطلوبة للفرز |

### قيمة الإرجاع

المؤشرات الأصلية (الموضع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى التحريك بواسطة عملية الفرز هذه، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // إنشاء أداة فرز البيانات
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // تحديد منطقة الفرز
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // تنفيذ الفرز
            dataSorter.Sort(worksheet.Cells, area);

            // احفظ المصنف
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

رتّب البيانات في النطاق.

```csharp
public int[] Sort()
```

### قيمة الإرجاع

المؤشرات الأصلية (الموضع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى التحريك بواسطة عملية الفرز هذه، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة للفرز
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // إنشاء كائن جدول/قائمة
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // فرز البيانات حسب العمود الأول
            table.AutoFilter.Sorter.Sort();

            // احفظ المصنف
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


