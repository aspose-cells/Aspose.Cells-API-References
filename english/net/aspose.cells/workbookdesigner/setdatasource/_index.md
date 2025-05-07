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
[Test]
        public void Method_ICellsDataTable_()
        {
            CustomerList customers = new CustomerList();
            customers.Add(new Customer("Thomas Hardy", "120 Hanover Sq., London"));
            customers.Add(new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino"));

            Workbook wb = new Workbook(Constants.sourcePath + "SmartMarker/CellsNet46927.xlsx");
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
// Called: designer.SetDataSource(dt);
[Test]
        public void Method_DataTable_()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(Constants.sourcePath + "CellsNet41180Template.xls");
            Workbook data = new Workbook(Constants.sourcePath + "CellsNet41180Data.xls");
            Cells dataCells = data.Worksheets[0].Cells;
            DataTable dt = dataCells.ExportDataTable(0, 0, dataCells.MaxRow + 1, dataCells.MaxColumn + 1, true);
            dt.TableName = "Data";
            designer.SetDataSource(dt);
            designer.Process();
            Cells rs = designer.Workbook.Worksheets[0].Cells;
            Assert.AreEqual(rs["C11"].Formula, "=SUBTOTAL(9,C7:C10)");
            Assert.AreEqual(rs["D11"].Formula, "=SUMPRODUCT(C7:C10,D7:D10)/SUM(C7:C10)");
            designer.Workbook.Save(Constants.destPath + "CellsNet41180dest.xls");
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
public static void Method_DataView_()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Workbook workbook = new Workbook(USBankConstants.sourcePath + "SmartMarkers3.xlsx");
            designer.Workbook = workbook;

            DataTable dt1 = CreateValidTable1();
            DataTable dt2 = CreateValidTable2();

            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            designer.Process(true);

            string output = USBankConstants.resultPath + "SmartMarkers_result.xlsx";
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
// Called: wd.SetDataSource(datasource.DefaultView);
[Test]
        public void Method_DataView_()
        {
            FileStream stream = File.OpenRead(Constants.sourcePath + "SmartMarker/CellsNet40073.xls");
            byte[] buffer = new byte[stream.Length];
            stream.Read(buffer, 0, buffer.Length);

            WorkbookDesigner wd = new WorkbookDesigner();
            using (MemoryStream templateStream = new MemoryStream(buffer))
            {
                wd.Workbook = new Workbook(templateStream);        //  Fetch template
                //wd.Workbook.Open(stream);
            }

            string[] smartmarkers = wd.GetSmartMarkers();

            DataTable datasource = new DataTable("COLORS_TIMES");

            datasource.Columns.Add("COLORS", typeof(string));
            datasource.Columns.Add("TIMES", typeof(DateTime));
            DateTime dt = DateTime.Now;
            datasource.Rows.Add(new object[] { "red", dt.AddDays(-1) });
            datasource.Rows.Add(new object[] { "yellow", dt });
            datasource.Rows.Add(new object[] { "green", dt.AddDays(+1) });

            wd.SetDataSource(datasource.DefaultView);

            wd.Process();
            Cells cells = wd.Workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells["A2"].StringValue, "red");
            Assert.AreEqual(cells["A4"].StringValue, "yellow");
            Assert.AreEqual(cells["A6"].StringValue, "green");
            Assert.AreEqual(cells["C1"].DoubleValue,CellsHelper.GetDoubleFromDateTime(dt,false));
            wd.Workbook.Save(Constants.destPath + "CellsNet40073.xls");

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
[Test]
        public void Method_Int32_()
        {
            string source = Constants.sourcePath + @"Database\Northwind.accdb";
            OleDbConnection con = new OleDbConnection("provider=Microsoft.ACE.OLEDB.12.0;data source=" + source);

            con.Open();

            OleDbCommand cmd = new OleDbCommand("Select * from Employees", con);

            IDataReader reader = cmd.ExecuteReader();

            WorkbookDesigner wd = new WorkbookDesigner();
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-45796.xls");
            wd.Workbook = wb;
            wd.SetDataSource("Employees", reader, 5);
            wd.Process(0, false);
            wd.SetDataSource("Employees", reader, 4);
            wd.Process(1, false);
            con.Close();
            wb.Save(Constants.destPath + "CELLSNET45796.xlsx");
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
// Called: myWorkbook.SetDataSource("Person", myList);
[Test]
        public void Method_Object_()
        {
            WorkbookDesigner myWorkbook = new WorkbookDesigner();
            //myWorkbook.Open(xlFileName);
            Worksheet curentWorksheet = myWorkbook.Workbook.Worksheets["Sheet1"];

            // Create temporary data
            IList<Person> myList = new List<Person>();
            myList.Add(new Person("X", 26));
            myList.Add(new Person("X", 32));
            myList.Add(new Person("Y", 19));


            // Set the headers and smart markers to the XL file
            curentWorksheet.Cells["A1"].PutValue("Name");
            curentWorksheet.Cells["B1"].PutValue("Age");
            curentWorksheet.Cells["A2"].PutValue("&=Person.Name(group:merge,skip:1)");
            curentWorksheet.Cells["B2"].PutValue("&=Person.Age");

            // Set the data to the XL sheet
            myWorkbook.SetDataSource("Person", myList);

            myWorkbook.Process();
            myWorkbook.Workbook.Save(Constants.destPath + "GroupCustomObjects.xls");
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


