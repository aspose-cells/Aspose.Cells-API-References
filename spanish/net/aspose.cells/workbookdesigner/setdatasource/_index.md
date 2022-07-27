---
title: SetDataSource
second_title: Referencia de API de Aspose.Cells para .NET
description: Establece la fuente de datos de unICellsDataTableaspose.cells/icellsdatatable objeto.
type: docs
weight: 120
url: /es/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Establece la fuente de datos de un[`ICellsDataTable`](../../icellsdatatable) objeto.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataSource | String | El nombre de la fuente de datos. |
| cellsDataTable | ICellsDataTable | tabla de datos. |

### Ver también

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Establece la fuente de datos de un objeto DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataSet | DataSet | Objeto de conjunto de datos |

### Ejemplos

```csharp

[C#]

//Cree un objeto de conexión, especifique la información del proveedor y configure la fuente de datos.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Abrir el objeto de conexión.
con.Open();
//Cree un objeto de comando y especifique la consulta SQL.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Cree un objeto de adaptador de datos.
OleDbDataAdapter da = new OleDbDataAdapter();
//Especifique el comando.
da.SelectCommand = cmd;
//Crear un objeto de conjunto de datos.
DataSet ds = new DataSet();
//Rellenar el conjunto de datos con los registros de la tabla.
da.Fill(ds, "Order Details");
//Crear una tabla de datos con respecto a la tabla del conjunto de datos.
DataTable dt = ds.Tables["Order Details"];
//Crear objeto WorkbookDesigner.
WorkbookDesigner wd = new WorkbookDesigner();
//Abra el archivo de plantilla (que contiene marcadores inteligentes).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
//Establecer la tabla de datos como fuente de datos.
wd.SetDataSource(dt);
//Procesar los marcadores inteligentes para completar los datos en las hojas de trabajo.
wd.Process(true);
//Guardar el archivo de Excel.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Cree un objeto de conexión, especifique la información del proveedor y configure la fuente de datos.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Abra el objeto de conexión.
con.Open()
'Cree un objeto de comando y especifique la consulta SQL.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Cree un objeto de adaptador de datos.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Especifique el comando.
da.SelectCommand = cmd
'Cree un objeto de conjunto de datos.
Dim ds As DataSet = New DataSet()
'Rellene el conjunto de datos con los registros de la tabla.
da.Fill(ds, "Order Details")
'Cree una tabla de datos con respecto a la tabla del conjunto de datos.
Dim dt As DataTable = ds.Tables("Order Details")
'Cree el objeto WorkbookDesigner.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Abra el archivo de plantilla (que contiene marcadores inteligentes).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Establezca la tabla de datos como la fuente de datos.
wd.SetDataSource(dt)
'Procese los marcadores inteligentes para completar los datos en las hojas de trabajo.
wd.Process(True)
'Guarde el archivo de Excel.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Establece la fuente de datos de un objeto DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataTable | DataTable | Objeto de tabla de datos |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Establece el origen de datos de un objeto DataView y lo vincula a un nombre de origen de datos.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataSourceName | String | Nombre de fuente de datos. |
| dataView | DataView | Objeto de vista de datos. |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Establece la fuente de datos de un objeto DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataView | DataView | objeto DataView |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Establece la fuente de datos de un objeto IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| name | String | El nombre del mapa de origen de datos. |
| dataReader | IDataReader | Objeto IDataReader |
| rowCount | Int32 | El número de filas de datos. Si el marcador inteligente no contiene "noadd", tenemos que insertar filas por el recuento de filas para problemas de rendimiento y fórmulas repetidas dinámicas. -1 significa que el parámetro es inútil. |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Establece el enlace de datos a una variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| variable | String | Nombre de variable creado con marcador inteligente. |
| data | Object | Datos fuente. |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Establece la fuente de datos de un objeto OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | OleDbConnection | Objeto OleDbConnection |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Establece el origen de datos de un objeto SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | SqlConnection | objeto SqlConnection |

### Ver también

* class [WorkbookDesigner](../../workbookdesigner)
* espacio de nombres [Aspose.Cells](../../workbookdesigner)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
