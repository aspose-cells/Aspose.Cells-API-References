---
title: Cells.ImportData
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Import data from custom data table
type: docs
url: /net/aspose.cells/cells/importdata/
---
## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Import data from custom data table.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ICellsDataTable | The custom data table. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
public void Cells_Method_ImportData()
{
    Workbook wb = new Workbook();

    ArrayList dataLists = new ArrayList();
    dataLists.Add(new object[] { "Name", "Age", "Gender" });
    dataLists.Add(new object[] { "Alice", 30, "Female" });
    dataLists.Add(new object[] { "Bob", 25, "Male" });
    dataLists.Add(new object[] { "Charlie", 35, "Male" });

    ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);

    wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
    Assert.AreEqual("Alice", wb.Worksheets[0].Cells["A2"].StringValue);

    wb.Worksheets.Add();
    wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
    Assert.AreEqual("Bob", wb.Worksheets[1].Cells["A3"].StringValue);
}
```

### See Also

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Import data from custom data table.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | DataTable | The DataTable object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |

### Return Value

Total number of rows imported.

### Examples

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Import data
DataTable dt = new DataTable("Products");
dt.Columns.Add("Product_ID",typeof(Int32));
dt.Columns.Add("Product_Name",typeof(string));
dt.Columns.Add("Units_In_Stock",typeof(Int32));
DataRow dr = dt.NewRow();
dr[0] = 1;
dr[1] = "Aniseed Syrup";
dr[2] = 15;
dt.Rows.Add(dr);
dr = dt.NewRow();
dr[0] = 2;
dr[1] = "Boston Crab Meat";
dr[2] = 123;
dt.Rows.Add(dr);
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
cells.ImportData(dt, 12, 12, options);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Import data
Dim dt as DataTable = new DataTable("Employee")
dt.Columns.Add("Employee_ID",typeof(Int32))
dt.Columns.Add("Employee_Name",typeof(string))
dt.Columns.Add("Gender",typeof(string))
Dim dr as DataRow = dt.NewRow()
dr(0) = 1
dr(1) = "John Smith"
dr(2) = "Male"
dt.Rows.Add(dr)
dr = dt.NewRow()
dr(0) = 2
dr(1) = "Mary Miller"
dr(2) = "Female"
dt.Rows.Add(dr)
Dim options as ImportTableOptions = new ImportTableOptions()
options.IsFieldNameShown = True
cells.ImportData(dt, 12, 12, options)

'Export data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Import data from data view.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |

### Return Value

Total number of rows imported.

### Examples

```csharp
// Called: cells.ImportData(dataview, 1048572, 16383, options);
public void Cells_Method_ImportData()
{
    caseName = "testImportDataColumn_Excel2007_007";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[1048572, 16383].PutValue(10);
    DataView dataview = getDataTable().DefaultView;
    ImportTableOptions options = new ImportTableOptions();
    options.ColumnIndexes = new int[] { 1 };
    options.IsFieldNameShown = false;
    options.InsertRows = true;

    cells.ImportData(dataview, 1048572, 16383, options);

    checkImportDataColumn_Excel2007_007(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xlsx");            
    workbook = new Workbook(Constants.destPath + "testImportDataColumn.xlsx");
    checkImportDataColumn_Excel2007_007(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xml", SaveFormat.SpreadsheetML );            
    workbook = new Workbook(Constants.destPath + "testImportDataColumn.xml");
    workbook.Save(Constants.destPath + "testImportDataColumn.xls");
}
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int) {#importdata_3}

Imports data from a IDataReader object.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| reader | IDataReader | The IDataReader object which contains data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### Return Value

Total number of rows imported.

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodImportDataWithIDataReaderInt32Int32Demo
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data table
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // Create IDataReader from DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Call ImportData method starting at cell A1 (row 0, column 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Auto-fit columns for better visibility
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Save the result
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Imports data from a IDataReader object.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| reader | IDataReader | The IDataReader object which contains data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | The options of importing table. |

### Return Value

Total number of rows imported.

### Examples

```csharp
// Called: int vNumberOfRowInsert = worksheet.Cells.ImportData(Reader1, 8, 0, options);
public void Cells_Method_ImportData()
{
    string path = Constants.sourcePath;
    Workbook dataWB = new Workbook(path + "example.xlsx");


    Worksheet dataWS = dataWB.Worksheets[0];


    DataTable dt = dataWS.Cells.ExportDataTable(0, 0, 25, 4, true);


    DataTableReader Reader1 = dt.CreateDataReader();


    Workbook workbook = new Workbook(path + "example.xls");


    Worksheet worksheet = workbook.Worksheets[0];

    ImportTableOptions options = new ImportTableOptions();
    options.IsFieldNameShown = false;
    options.InsertRows = true;
    options.ConvertNumericData = false;
    options.DateFormat = "dd/MM/yyyy";
  //  options.TotalRows = dt.Rows.Count;

    int vNumberOfRowInsert = worksheet.Cells.ImportData(Reader1, 8, 0, options);
    Assert.AreEqual(worksheet.Cells["A35"].StringValue, "New Members");
}
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


