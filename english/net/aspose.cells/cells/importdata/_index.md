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
// Called: sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
public static void Method_ImportTableOptions_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            List&lt;CustomData&gt; dataList = new List&lt;CustomData&gt;
            {
                new CustomData { Id = 1, Name = &quot;John Doe&quot;, Age = 30 },
                new CustomData { Id = 2, Name = &quot;Jane Smith&quot;, Age = 25 },
                new CustomData { Id = 3, Name = &quot;Sam Brown&quot;, Age = 35 }
            };

            // Get the CellsDataTableFactory instance from the workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Create an ICellsDataTable instance from the custom data list
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Import the data table into the worksheet starting at cell A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Save the workbook
            workbook.Save(&quot;CellsDataTableFactoryDemo.xlsx&quot;);
            workbook.Save(&quot;CellsDataTableFactoryDemo.pdf&quot;);
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
// Called: cells.ImportData(dataview, 0, 0, new ImportTableOptions()
[Test]
        public void Method_ImportTableOptions_()
        {
            caseName = &quot;testImportDataView_021&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells[0, 0].PutValue(10);
            cells.ImportData(dataview, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = false,
                InsertRows = true,
                TotalRows = 2,
                TotalColumns = 2,
                NumberFormats = BuildNumberFormats(&quot;0.00&quot;, 2)
            });

            checkImportDataView_021(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xls&quot;);
            checkImportDataView_021(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + &quot;testDataView.xlsx&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xlsx&quot;);
            checkImportDataView_021(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + &quot;testDataView.xml&quot;, SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xml&quot;);
            checkImportDataView_021(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);
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
            Workbook dataWB = new Workbook(path + &quot;Cellsnet43333_sampleData.xlsx&quot;);


            Worksheet dataWS = dataWB.Worksheets[0];


            DataTable dt = dataWS.Cells.ExportDataTable(0, 0, 25, 4, true);


            DataTableReader Reader1 = dt.CreateDataReader();


            Workbook workbook = new Workbook(path + &quot;Cellsnet43333_AdjustForm.xls&quot;);


            Worksheet worksheet = workbook.Worksheets[0];

            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = false;
            options.InsertRows = true;
            options.ConvertNumericData = false;
            options.DateFormat = &quot;dd/MM/yyyy&quot;;
          //  options.TotalRows = dt.Rows.Count;

            int vNumberOfRowInsert = worksheet.Cells.ImportData(Reader1, 8, 0, options);
            Assert.AreEqual(worksheet.Cells[&quot;A35&quot;].StringValue, &quot;New Members&quot;);
        }
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


