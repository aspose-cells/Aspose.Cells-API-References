---
title: SetDataSource
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 120
url: /net/aspose.cells/workbookdesigner/setdatasource/
---
## WorkbookDesigner.SetDataSource method (1 of 8)

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
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=d:\\test\\Northwind.mdb");
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
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=d:\test\Northwind.mdb")
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

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (2 of 8)

Sets data source of a DataTable object.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | DataTable object |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (3 of 8)

Sets data source of a [`ICellsDataTable`](../../icellsdatatable) object.

```csharp
public void SetDataSource(string name, ICellsDataTable dataTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the table. |
| dataTable | ICellsDataTable | DataTable object |

### See Also

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (4 of 8)

Sets data source of a DataView object and binds it to a data source name.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataSourceName | String | Data source name. |
| dataView | DataView | DataView object. |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (5 of 8)

Sets data source of a DataView object.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | DataView object |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (6 of 8)

Sets data source of a IDataReader object.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The data source map name. |
| dataReader | IDataReader | IDataReader object |
| rowCount | Int32 | The number of the data rows. If the smart marker does not contains "noadd", we have to insert rows by the row count for performance issue and dynamic repeated formulas. -1 means the param is useless. |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (7 of 8)

Sets data binding to a variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| data | Object | Source data. |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner.SetDataSource method (8 of 8)

Sets data array binding to a variable.

```csharp
public void SetDataSource(string variable, object[] dataArray)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| dataArray | Object[] | Source data array. |

### See Also

* class [WorkbookDesigner](../../workbookdesigner)
* namespace [Aspose.Cells](../../workbookdesigner)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
