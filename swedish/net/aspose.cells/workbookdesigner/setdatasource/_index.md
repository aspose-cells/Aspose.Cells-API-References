---
title: SetDataSource
second_title: Aspose.Cells för .NET API-referens
description: Anger datakälla för enICellsDataTableaspose.cells/icellsdatatable objekt.
type: docs
weight: 120
url: /sv/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Anger datakälla för en[`ICellsDataTable`](../../icellsdatatable) objekt.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSource | String | Namnet på datakällan. |
| cellsDataTable | ICellsDataTable | datatabell. |

### Se även

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Anger datakälla för ett DataSet-objekt.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSet | DataSet | DataSet-objekt |

### Exempel

```csharp

[C#]

//Skapa ett anslutningsobjekt, ange leverantörsinformation och ställ in datakällan.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Öppna anslutningsobjektet.
con.Open();
//Skapa ett kommandoobjekt och ange SQL-frågan.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Skapa ett dataadapterobjekt.
OleDbDataAdapter da = new OleDbDataAdapter();
//Ange kommandot.
da.SelectCommand = cmd;
//Skapa ett datasetobjekt.
DataSet ds = new DataSet();
//Fyll datasetet med tabellposterna.
da.Fill(ds, "Order Details");
//Skapa en datatabell med avseende på datasettabellen.
DataTable dt = ds.Tables["Order Details"];
//Skapa WorkbookDesigner-objekt.
WorkbookDesigner wd = new WorkbookDesigner();
//Öppna mallfilen (som innehåller smarta markörer).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
//Ställ in datatabellen som datakälla.
wd.SetDataSource(dt);
//Bearbeta de smarta markörerna för att fylla i data i kalkylbladen.
wd.Process(true);
//Spara excel-filen.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Skapa ett anslutningsobjekt, ange leverantörsinformation och ställ in datakällan.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Öppna anslutningsobjektet.
con.Open()
'Skapa ett kommandoobjekt och ange SQL-frågan.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Skapa ett dataadapterobjekt.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Ange kommandot.
da.SelectCommand = cmd
'Skapa ett datauppsättningsobjekt.
Dim ds As DataSet = New DataSet()
'Fyll datauppsättningen med tabellposterna.
da.Fill(ds, "Order Details")
'Skapa en datatabell med avseende på datauppsättningstabell.
Dim dt As DataTable = ds.Tables("Order Details")
'Skapa WorkbookDesigner-objekt.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Öppna mallfilen (som innehåller smarta markörer).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Ställ in datatabellen som datakälla.
wd.SetDataSource(dt)
'Bearbeta de smarta markörerna för att fylla data i kalkylbladen.
wd.Process(True)
'Spara excel-filen.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Anger datakälla för ett DataTable-objekt.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataTable | DataTable | DataTable-objekt |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Anger datakälla för ett DataView-objekt och binder det till ett datakällas namn.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSourceName | String | Datakällans namn. |
| dataView | DataView | DataView-objekt. |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Anger datakälla för ett DataView-objekt.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataView | DataView | DataView-objekt |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Anger datakälla för ett IDataReader-objekt.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Datakällans kartnamn. |
| dataReader | IDataReader | IDataReader-objekt |
| rowCount | Int32 | Antalet datarader. Om den smarta markören inte innehåller "noadd", måste vi infoga rader efter radantal för prestandaproblem och dynamiska upprepade formler. -1 betyder att paramet är värdelöst. |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Anger databindning till en variabel.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| variable | String | Variabelnamn skapat med smart markör. |
| data | Object | Källdata. |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Anger datakälla för ett OleDbConnection-objekt.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection-objekt |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Anger datakälla för ett SqlConnection-objekt.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection-objekt |

### Se även

* class [WorkbookDesigner](../../workbookdesigner)
* namnutrymme [Aspose.Cells](../../workbookdesigner)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
