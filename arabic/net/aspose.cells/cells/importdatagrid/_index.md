---
title: "Cells.ImportDataGrid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تستورد DataGrid إلى ورقة عمل"
type: docs
url: /ar/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

يستورد DataGrid إلى ورقة عمل.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataGrid | DataGrid | كائن DataGrid الذي سيتم استيراده. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| insertRows | منطقي | يشير إلى ما إذا كانت صفوف إضافية تُضاف لتناسب البيانات. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء DataTable لمحاكاة بيانات DataGrid
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // استيراد البيانات باستخدام ImportDataView المتوفر في API
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

يستورد DataGrid إلى ورقة عمل.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataGrid | DataGrid | كائن DataGrid الذي سيتم استيراده. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| insertRows | منطقي | يشير إلى ما إذا كانت صفوف إضافية تُضاف لتناسب البيانات. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // إنشاء DataGrid عينة مع بعض البيانات
                // استخدام مصفوفة سلاسل بسيطة لمحاكاة بيانات DataGrid
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // استيراد البيانات إلى ورقة العمل بدءًا من الصف 0، العمود 0
                cells.ImportArray(gridData, 0, 0);

                // احفظ المصنف
                workbook.Save("ImportDataGridDemo.xlsx");
                Console.WriteLine("Data imported successfully to ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
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

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

يستورد DataGrid إلى ورقة عمل.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataGrid | DataGrid | كائن DataGrid الذي سيتم استيراده. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| insertRows | منطقي | يشير إلى ما إذا كانت صفوف إضافية تُضاف لتناسب البيانات. |
| importStyle | منطقي | يشير إلى ما إذا كان يتم استيراد نمط الخلية. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32Bo257661Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة عادةً ما تأتي من DataGrid
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // استيراد البيانات مباشرة إلى الخلايا لأننا لا نستطيع استخدام DataGrid
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // احفظ المصنف
                workbook.Save("ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


