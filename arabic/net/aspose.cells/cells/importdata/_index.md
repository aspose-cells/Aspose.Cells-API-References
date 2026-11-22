---
title: "Cells.ImportData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تستورد البيانات من كائن IDataReader"
type: docs
url: /ar/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

يستورد البيانات من كائن IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| القارئ | IDataReader | كائن IDataReader الذي يحتوي على البيانات. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء جدول بيانات تجريبي
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // إنشاء IDataReader من DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // استدعاء طريقة ImportData بدءًا من الخلية A1 (الصف 0، العمود 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // ضبط الأعمدة تلقائيًا لتحسين الرؤية
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

يستورد البيانات من كائن IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| القارئ | IDataReader | كائن IDataReader الذي يحتوي على البيانات. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| خيارات | ImportTableOptions | خيارات استيراد الجدول. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithIDataReaderInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            // أنشئ DataTable نموذجية
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // أضف بيانات تجريبية
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // إنشاء DataTableReader
            DataTableReader reader = dt.CreateDataReader();

            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين خيارات الاستيراد
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // استيراد البيانات بدءًا من الصف 5، العمود 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // احفظ المصنف
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

استيراد البيانات من جدول بيانات مخصص.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | ICellsDataTable | جدول البيانات المخصص. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| خيارات | ImportTableOptions | خيارات الاستيراد |

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithICellsDataTableInt32Int32ImporDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { "Name", "Age", "Gender" });
            dataLists.Add(new object[] { "Alice", 30, "Female" });
            dataLists.Add(new object[] { "Bob", 25, "Male" });
            dataLists.Add(new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            
            Console.WriteLine("Data imported to first worksheet:");
            Console.WriteLine(wb.Worksheets[0].Cells["A2"].StringValue);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

استيراد البيانات من جدول بيانات مخصص.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | DataTable | كائن DataTable المراد استيراده. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| خيارات | ImportTableOptions | خيارات الاستيراد |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataTableInt32Int32ImportTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء DataTable نموذجي
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // أضف بيانات تجريبية
            DataRow row = dataTable.NewRow();
            row[0] = 1;
            row[1] = "Aniseed Syrup";
            row[2] = 15;
            dataTable.Rows.Add(row);

            row = dataTable.NewRow();
            row[0] = 2;
            row[1] = "Boston Crab Meat";
            row[2] = 123;
            dataTable.Rows.Add(row);

            // تعيين خيارات الاستيراد
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // استيراد البيانات بدءًا من الصف 5، العمود 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // احفظ المصنف
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

استيراد البيانات من DataView.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataView | DataView | كائن DataView المراد استيراده. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| خيارات | ImportTableOptions | خيارات الاستيراد |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataViewInt32Int32ImportTableODemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء جدول بيانات تجريبي
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // أضف بيانات تجريبية
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // إنشاء ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // استيراد البيانات من DataView إلى الخلايا بدءًا من الصف 0، العمود 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // احفظ المصنف
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


