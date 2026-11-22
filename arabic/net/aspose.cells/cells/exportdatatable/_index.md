---
title: "Cells.ExportDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تصدر البيانات في مجموعة Cells إلى كائن DataTable"
type: docs
url: /ar/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### ملاحظات

إذا استخدمت هذه الطريقة لتصدير كتلة من البيانات، يرجى التأكد من أن البيانات في العمود يجب أن تكون من نفس نوع البيانات. وإلا، استخدم طريقة [`ExportDataTableAsString`](../exportdatatableasstring/) بدلاً من ذلك.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // تصدير البيانات إلى DataTable (بدءًا من الصف 0، العمود 0، مع 5 صفوف و3 أعمدة)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // عرض البيانات المصدرة
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| exportColumnName | منطقي | يشير إلى ما إذا كانت البيانات في الصف الأول تُصدّر إلى اسم العمود في DataTable. |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // تصدير البيانات إلى DataTable (الصف الأول يحتوي على رؤوس الأعمدة)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // عرض البيانات المصدرة
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| خيارات | ExportTableOptions | جميع خيارات تصدير الجدول |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // تعيين القيمة والتنسيق للخلية A1
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // إنشاء خيارات التصدير
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // تصدير باستخدام استراتيجية تنسيق CellStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // تصدير باستخدام استراتيجية تنسيق None
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // تصدير باستخدام استراتيجية تنسيق DisplayStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


