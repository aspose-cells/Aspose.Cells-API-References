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
// Called: designer.SetDataSource(&amp;quot;Customer&amp;quot;, new CustomerDataSource(customers));
[Test]
        public void Method_ICellsDataTable_()
        {
            CustomerList customers = new CustomerList();
            customers.Add(new Customer(&quot;Thomas Hardy&quot;, &quot;120 Hanover Sq., London&quot;));
            customers.Add(new Customer(&quot;Paolo Accorti&quot;, &quot;Via Monte Bianco 34, Torino&quot;));

            Workbook wb = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsNet46927.xlsx&quot;);
            WorkbookDesigner designer = new WorkbookDesigner(wb);

            //  designer.SetDataSource(&quot;Customer&quot;, customers);
            designer.SetDataSource(&quot;Customer&quot;, new CustomerDataSource(customers));
            designer.Process();
            wb.Save(Constants.destPath + &quot;dest.xlsx&quot;);
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
// Called: wbd.SetDataSource(dataTable);
[Test]
        public void Method_DataTable_()
        {
            var wbd = new WorkbookDesigner();
            wbd.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsNet46057.xlsx&quot;);

            var dataTable = new DataTable(&quot;TableA&quot;);
            dataTable.Columns.Add(&quot;ColumnA&quot;);
            dataTable.Columns.Add(&quot;ColumnB&quot;);

            for (var i = 0; i &lt; 5; i++)
            {
                var dr = dataTable.NewRow();
                dr[&quot;ColumnA&quot;] = &quot;ColumnA Value&quot; + i;
                dr[&quot;ColumnB&quot;] = &quot;ColumnB Value&quot; + i;
                dataTable.Rows.Add(dr);
            }

            wbd.SetDataSource(dataTable);

            wbd.Process();
            Assert.AreEqual(&quot;=Sheet1!$A$1:$B$5&quot;,wbd.Workbook.Worksheets.Names[0].RefersTo);

            wbd.Workbook.Save(Constants.destPath + &quot;CellsNet46057.xlsx&quot;);
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
// Called: wd.SetDataSource(&amp;quot;dataSourceName&amp;quot;, new DataView(dt));
public static void Method_DataView_()
        {
            // Create WorkbookDesigner object
            WorkbookDesigner wd = new WorkbookDesigner();

            // Open the template file (which contains smart markers)
            wd.Workbook = new Workbook(&quot;SmartMarker_Designer_original.xlsx&quot;);

            // Initialize your data from data source
            DataSet ds = new DataSet();
            // Add data to the dataset (this is just an example, replace with actual data source)
            DataTable dt = new DataTable(&quot;Table1&quot;);
            dt.Columns.Add(&quot;Column1&quot;);
            dt.Columns.Add(&quot;Column2&quot;);
            dt.Rows.Add(&quot;Value1&quot;, &quot;Value2&quot;);
            dt.Rows.Add(&quot;Value11&quot;, &quot;Value22&quot;);
            ds.Tables.Add(dt);

            // Set the dataset as the data source
            wd.SetDataSource(ds);

            // Process the smart markers to fill the data into the worksheets
            wd.Process(true);

            // Save the excel file
            wd.Workbook.Save(&quot;WorkbookDesignerExample.xlsx&quot;);

            // Demonstrating other properties
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Clear data source
            wd.ClearDataSource();

            // Set data source using different methods
            wd.SetDataSource(&quot;dataSourceName&quot;, dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource(&quot;dataSourceName&quot;, new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource(&quot;name&quot;, new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource(&quot;variable&quot;, &quot;{\&quot;key\&quot;:\&quot;value\&quot;}&quot;);
            wd.SetDataSource(&quot;variable&quot;, new object());

            // Process the smart markers again
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Save the excel file again
            wd.Workbook.Save(&quot;WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx&quot;);

            return;
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
            FileStream stream = File.OpenRead(Constants.sourcePath + &quot;SmartMarker/CellsNet40073.xls&quot;);
            byte[] buffer = new byte[stream.Length];
            stream.Read(buffer, 0, buffer.Length);

            WorkbookDesigner wd = new WorkbookDesigner();
            using (MemoryStream templateStream = new MemoryStream(buffer))
            {
                wd.Workbook = new Workbook(templateStream);        //  Fetch template
                //wd.Workbook.Open(stream);
            }

            string[] smartmarkers = wd.GetSmartMarkers();

            DataTable datasource = new DataTable(&quot;COLORS_TIMES&quot;);

            datasource.Columns.Add(&quot;COLORS&quot;, typeof(string));
            datasource.Columns.Add(&quot;TIMES&quot;, typeof(DateTime));
            DateTime dt = DateTime.Now;
            datasource.Rows.Add(new object[] { &quot;red&quot;, dt.AddDays(-1) });
            datasource.Rows.Add(new object[] { &quot;yellow&quot;, dt });
            datasource.Rows.Add(new object[] { &quot;green&quot;, dt.AddDays(+1) });

            wd.SetDataSource(datasource.DefaultView);

            wd.Process();
            Cells cells = wd.Workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;A2&quot;].StringValue, &quot;red&quot;);
            Assert.AreEqual(cells[&quot;A4&quot;].StringValue, &quot;yellow&quot;);
            Assert.AreEqual(cells[&quot;A6&quot;].StringValue, &quot;green&quot;);
            Assert.AreEqual(cells[&quot;C1&quot;].DoubleValue,CellsHelper.GetDoubleFromDateTime(dt,false));
            wd.Workbook.Save(Constants.destPath + &quot;CellsNet40073.xls&quot;);

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
// Called: wd.SetDataSource(&amp;quot;Employees&amp;quot;, reader, 4);
[Test]
        public void Method_Int32_()
        {
            string source = Constants.sourcePath + @&quot;Database\Northwind.accdb&quot;;
            OleDbConnection con = new OleDbConnection(&quot;provider=Microsoft.ACE.OLEDB.12.0;data source=&quot; + source);

            con.Open();

            OleDbCommand cmd = new OleDbCommand(&quot;Select * from Employees&quot;, con);

            IDataReader reader = cmd.ExecuteReader();

            WorkbookDesigner wd = new WorkbookDesigner();
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-45796.xls&quot;);
            wd.Workbook = wb;
            wd.SetDataSource(&quot;Employees&quot;, reader, 5);
            wd.Process(0, false);
            wd.SetDataSource(&quot;Employees&quot;, reader, 4);
            wd.Process(1, false);
            con.Close();
            wb.Save(Constants.destPath + &quot;CELLSNET45796.xlsx&quot;);
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
// Called: designer.SetDataSource(&amp;quot;Person&amp;quot;, list);
[Test]
        public void Method_Object_()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CellsNet13728.xls&quot;);
            //designer.Open(Constants.sourcePath +&quot;CellsNet13728.xls&quot;);

          
            ArrayList list = new ArrayList();
            //list.Add(new Person(&quot;simon&quot;, 30));
            //list.Add(new Person(&quot;Johnson&quot;, 33));
            list.Add(new CustomDataRow());
            list.Add(new CustomDataRow());
            designer.SetDataSource(&quot;Person&quot;, list);
            designer.Process(false);

            Assert.AreEqual(designer.Workbook.Worksheets[1].Cells[&quot;B2&quot;].StringValue, &quot;John&quot;);
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


