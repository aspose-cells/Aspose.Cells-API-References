---
title: SetDataSource
second_title: Aspose.Cells for .NET API 参考
description: 设置ICellsDataTableaspose.cells/icellsdatatable对象的数据源
type: docs
weight: 120
url: /zh/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

设置[`ICellsDataTable`](../../icellsdatatable)对象的数据源。

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dataSource | String | 数据源的名称。 |
| cellsDataTable | ICellsDataTable | 数据表。 |

### 也可以看看

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

设置 DataSet 对象的数据源。

```csharp
public void SetDataSource(DataSet dataSet)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dataSet | DataSet | 数据集对象 |

### 例子

```csharp

[C#]

 //创建连接对象，指定提供者信息并设置数据源。
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
 //打开连接对象.
con.Open();
 //创建命令对象并指定SQL查询。
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
 //创建一个数据适配器对象.
OleDbDataAdapter da = new OleDbDataAdapter();
 //指定命令.
da.SelectCommand = cmd;
 //创建一个数据集对象.
DataSet ds = new DataSet();
 //用表记录填充数据集.
da.Fill(ds, "Order Details");
 //根据数据集表创建一个数据表。
DataTable dt = ds.Tables["Order Details"];
 //创建WorkbookDesigner对象.
WorkbookDesigner wd = new WorkbookDesigner();
 //打开模板文件（包含智能标记）.
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
 //设置数据表为数据源.
wd.SetDataSource(dt);
 //处理智能标记以将数据填充到工作表中。
wd.Process(true);
 //保存excel文件.
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

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

设置 DataTable 对象的数据源。

```csharp
public void SetDataSource(DataTable dataTable)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dataTable | DataTable | 数据表对象 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

设置 DataView 对象的数据源并将其绑定到数据源名称。

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dataSourceName | String | 数据源名称。 |
| dataView | DataView | DataView 对象。 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

设置 DataView 对象的数据源。

```csharp
public void SetDataSource(DataView dataView)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dataView | DataView | DataView 对象 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

设置 IDataReader 对象的数据源。

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 数据源映射名称。 |
| dataReader | IDataReader | IDataReader 对象 |
| rowCount | Int32 | 数据行数。 如果智能标记不包含“noadd”， 我们必须按行数插入行，以解决性能问题和动态重复公式。 -1 表示参数无用。 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

将数据绑定设置为变量。

```csharp
public void SetDataSource(string variable, object data)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| variable | String | 使用智能标记创建的变量名称。 |
| data | Object | 源数据。 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

设置 OleDbConnection 对象的数据源。

```csharp
public void SetDataSource(OleDbConnection connection)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection 对象 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

设置 SqlConnection 对象的数据源。

```csharp
public void SetDataSource(SqlConnection connection)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection 对象 |

### 也可以看看

* class [WorkbookDesigner](../../workbookdesigner)
* 命名空间 [Aspose.Cells](../../workbookdesigner)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
