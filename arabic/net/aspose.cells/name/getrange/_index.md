---
title: "Name.GetRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Name. تحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق"
type: docs
url: /ar/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق.

```csharp
public Range GetRange()
```

### قيمة الإرجاع

النطاق.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // أظهر طريقة GetRange
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // عدّل النطاق
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // احفظ المصنف
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق

```csharp
public Range GetRange(bool recalculate)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | منطقي | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

### قيمة الإرجاع

النطاق.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء بيانات عينة
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // أنشئ نطاقًا مسمىً مع صيغة
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // استخدم النطاق المسمى في الصيغ
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // حساب الصيغ
            wb.CalculateFormula();

            // احصل على النطاق باستخدام GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // أنشئ مخططًا باستخدام النطاق المسمى
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. إذا لم تكن إشارة هذا الاسم مطلقة، قد يكون النطاق مختلفًا لخلايا مختلفة.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة المقابل. |
| صف | Int32 | فهرس الصف المقابل. |
| عمود | Int32 | فهرس العمود المقابل |

### قيمة الإرجاع

النطاق.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // أنشئ نطاقًا مسمىً باستخدام توقيع الطريقة الصحيح
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // احصل على النطاق باستخدام GetRange مع معلمات الصف والعمود وعدد الصفوف
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // اعرض مرجع النطاق
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


