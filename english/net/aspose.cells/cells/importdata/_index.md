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
[Test]
        public void Method_ImportTableOptions_()
        {
            Workbook wb = new Workbook();

            object[][] data = new object[4][];
            data[0] = new object[] { "Name", "Age", "Gender" };
            data[1] = (new object[] { "Alice", 30, "Female" });
            data[2] = (new object[] { "Bob", 25, "Male" });
            data[3] = (new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(data, true,null);

            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Assert.AreEqual("Alice", wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportObjectArray(data, 0, 0, true);
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
// Called: cells.ImportData(dataview, 1048574, 0, new ImportTableOptions()
[Test]
        public void Method_ImportTableOptions_()
        {
            caseName = "testImportDataView_Excel2007_009";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells[1048574, 0].PutValue(10);
            cells.ImportData(dataview, 1048574, 0, new ImportTableOptions()
            { IsFieldNameShown = false, InsertRows = false, TotalRows = 1, TotalColumns = 2 });

            checkImportDataView_Excel2007_009(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "testDataView.xlsx");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
            checkImportDataView_Excel2007_009(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + "testDataView.xml", SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + "testDataView.xml");
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");
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
[Test]
        public void Method_ImportTableOptions_()
        {
            string path = Constants.sourcePath;
            Workbook dataWB = new Workbook(path + "Cellsnet43333_sampleData.xlsx");


            Worksheet dataWS = dataWB.Worksheets[0];


            DataTable dt = dataWS.Cells.ExportDataTable(0, 0, 25, 4, true);


            DataTableReader Reader1 = dt.CreateDataReader();


            Workbook workbook = new Workbook(path + "Cellsnet43333_AdjustForm.xls");


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


