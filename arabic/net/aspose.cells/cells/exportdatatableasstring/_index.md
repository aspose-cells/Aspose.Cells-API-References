---
title: "Cells.ExportDataTableAsString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تصدر البيانات في مجموعة Cells إلى كائن DataTable"
type: docs
url: /ar/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
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

جميع البيانات في مجموعة [`Cells`](../) تُحوَّل إلى سلاسل نصية.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية إلى الخلايا
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // تصدير البيانات إلى DataTable كسلاسل نصية
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // عرض البيانات المصدرة
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
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

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
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

### ملاحظات

جميع البيانات في مجموعة [`Cells`](../) تُحوَّل إلى سلاسل نصية.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
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

            // تصدير البيانات إلى DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // عرض البيانات المصدرة
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


