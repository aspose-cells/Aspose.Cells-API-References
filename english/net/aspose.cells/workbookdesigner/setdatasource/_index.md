---
title: WorkbookDesigner.SetDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Sets data source of a ICellsDataTable object
type: docs
url: /net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Sets data source of a [`ICellsDataTable`](../../icellsdatatable/) object.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataSource | String | The name of the data source. |
| cellsDataTable | ICellsDataTable | data table. |

### Examples

```csharp
// Called: designer.SetDataSource("Customer", new CustomerDataSource(customers));
public void WorkbookDesigner_Method_SetDataSource()
{
    CustomerList customers = new CustomerList();
    customers.Add(new Customer("Thomas Hardy", "120 Hanover Sq., London"));
    customers.Add(new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino"));

    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    WorkbookDesigner designer = new WorkbookDesigner(wb);

    //  designer.SetDataSource("Customer", customers);
    designer.SetDataSource("Customer", new CustomerDataSource(customers));
    designer.Process();
    wb.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Sets data source of a DataSet object.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataSet | DataSet | DataSet object |

### Examples

```csharp

[C#]

//Create a connection object, specify the provider info and set the data source.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Open the connection object.
con.Open();
//Create a command object and specify the SQL query.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Create a data adapter object.
OleDbDataAdapter da = new OleDbDataAdapter();
//Specify the command.
da.SelectCommand = cmd;
//Create a dataset object.
DataSet ds = new DataSet();
//Fill the dataset with the table records.
da.Fill(ds, "Order Details");
//Create a datatable with respect to dataset table.
DataTable dt = ds.Tables["Order Details"];
//Create WorkbookDesigner object.
WorkbookDesigner wd = new WorkbookDesigner();
//Open the template file (which contains smart markers).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
//Set the datatable as the data source.
wd.SetDataSource(dt);
//Process the smart markers to fill the data into the worksheets.
wd.Process(true);
//Save the excel file.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Create a connection object, specify the provider info and set the data source.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Open the connection object.
con.Open()
'Create a command object and specify the SQL query.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Create a data adapter object.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Specify the command.
da.SelectCommand = cmd
'Create a dataset object.
Dim ds As DataSet = New DataSet()
'Fill the dataset with the table records.
da.Fill(ds, "Order Details")
'Create a datatable with respect to dataset table.
Dim dt As DataTable = ds.Tables("Order Details")
'Create WorkbookDesigner object.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Open the template file (which contains smart markers).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Set the datatable as the data source.
wd.SetDataSource(dt)
'Process the smart markers to fill the data into the worksheets.
wd.Process(True)
'Save the excel file.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Sets data source of a DataTable object.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | DataTable object |

### Examples

```csharp
// Called: wbd2.SetDataSource(dataTable);
public void WorkbookDesigner_Method_SetDataSource()
{
    var wbd2 = new WorkbookDesigner();
    wbd2.Workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    var dataTable = new DataTable("Table1");
    dataTable.Columns.Add("Category");
    dataTable.Columns.Add("ColumnA");

    for (var i = 0; i < 5; i++)
    {
        var dr = dataTable.NewRow();
        dr["Category"] = "Category" + i;
        dr["ColumnA"] = "Value" + i;
        dataTable.Rows.Add(dr);
    }

    wbd2.SetDataSource(dataTable);

    wbd2.Process();
    Assert.IsTrue(wbd2.Workbook.Worksheets[0].Cells["A8"].IsMerged);
    wbd2.Workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Sets data source of a DataView object and binds it to a data source name.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataSourceName | String | Data source name. |
| dataView | DataView | DataView object. |

### Examples

```csharp
// Called: designer.SetDataSource("Remaining", dt2.DefaultView);
public void WorkbookDesigner_Method_SetDataSource()
{
WorkbookDesigner designer = new WorkbookDesigner();
Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    designer.Workbook = workbook;

    DataTable dt1 = CreateValidTable1_31068();
    DataTable dt2 = CreateValidTable2_31068();

    designer.SetDataSource("Investment", dt1.DefaultView);
    designer.SetDataSource("Remaining", dt2.DefaultView);

    designer.Process(true);
    Assert.AreEqual(workbook.Worksheets[0].Cells["B1"].StringValue, "Id number 2");
    string output = Constants.destPath + "example.xlsx";
    workbook.Save(output);
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Sets data source of a DataView object.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | DataView object |

### Examples

```csharp
// Called: wd.SetDataSource(new DataView(dt));
public static void WorkbookDesigner_Method_SetDataSource()
        {
            // Create WorkbookDesigner object
            WorkbookDesigner wd = new WorkbookDesigner();

            // Open the template file (which contains smart markers)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Initialize your data from data source
            DataSet ds = new DataSet();
            // Add data to the dataset (this is just an example, replace with actual data source)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Set the dataset as the data source
            wd.SetDataSource(ds);

            // Process the smart markers to fill the data into the worksheets
            wd.Process(true);

            // Save the excel file
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Demonstrating other properties
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Clear data source
            wd.ClearDataSource();

            // Set data source using different methods
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Process the smart markers again
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Save the excel file again
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Sets data source of a IDataReader object.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The data source map name. |
| dataReader | IDataReader | IDataReader object |
| rowCount | Int32 | The number of the data rows. If the smart marker does not contains "noadd", we have to insert rows by the row count for performance issue and dynamic repeated formulas. -1 means the param is useless. |

### Examples

```csharp
// Called: wd.SetDataSource("Employees", reader, 5);
public void WorkbookDesigner_Method_SetDataSource()
{
    string source = Constants.sourcePath + @"Database\Northwind.accdb";
    OleDbConnection con = new OleDbConnection("provider=Microsoft.ACE.OLEDB.12.0;data source=" + source);

    con.Open();

    OleDbCommand cmd = new OleDbCommand("Select * from Employees", con);

    IDataReader reader = cmd.ExecuteReader();

    WorkbookDesigner wd = new WorkbookDesigner();
    Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
    wd.Workbook = wb;
    wd.SetDataSource("Employees", reader, 5);
    wd.Process(0, false);
    wd.SetDataSource("Employees", reader, 4);
    wd.Process(1, false);
    con.Close();
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Sets data binding to a variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| data | Object | Source data. |

### Examples

```csharp
// Called: designer.SetDataSource("Person", list);
public void WorkbookDesigner_Method_SetDataSource()
{
    WorkbookDesigner designer = new WorkbookDesigner();
    //designer.Open(Constants.sourcePath + "example.xls");
    designer.Workbook = new Workbook(Constants.sourcePath + "example.xls");
    System.Collections.Generic.ICollection<Person> list = new System.Collections.Generic.List<Person>();
    Person simon = new Person("simon", 30);
    simon.Wife = new Wife("simon.wife", 30);
    Person Johnson = new Person("Johnson", 30);
    Johnson.Wife = new Wife("Johnson.wife", 30);
    list.Add(simon);
    list.Add(Johnson);
    designer.SetDataSource("Person", list);
    designer.Process(false);
    Cells cells = designer.Workbook.Worksheets["Sheet1"].Cells;
    Assert.AreEqual(cells["A1"].StringValue, "simon");
    Assert.AreEqual(cells["A2"].StringValue, "Johnson");
    Assert.AreEqual(cells["C1"].StringValue, "simon.wife");
    Assert.AreEqual(cells["C2"].StringValue, "Johnson.wife");
    designer.Workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Sets data source of a OleDbConnection object.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection object |

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Sets data source of a SqlConnection object.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection object |

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


