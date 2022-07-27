---
title: SetDataSource
second_title: Aspose.Cells für .NET-API-Referenz
description: Legt die Datenquelle von a festICellsDataTableaspose.cells/icellsdatatable Objekt.
type: docs
weight: 120
url: /de/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Legt die Datenquelle von a fest[`ICellsDataTable`](../../icellsdatatable) Objekt.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSource | String | Der Name der Datenquelle. |
| cellsDataTable | ICellsDataTable | Datentabelle. |

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Legt die Datenquelle eines DataSet-Objekts fest.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSet | DataSet | DataSet-Objekt |

### Beispiele

```csharp

[C#]

//Erstellen Sie ein Verbindungsobjekt, geben Sie die Anbieterinformationen an und legen Sie die Datenquelle fest.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Öffne das Verbindungsobjekt.
con.Open();
//Ein Befehlsobjekt erstellen und die SQL-Abfrage angeben.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Ein Datenadapterobjekt erstellen.
OleDbDataAdapter da = new OleDbDataAdapter();
//Geben Sie den Befehl an.
da.SelectCommand = cmd;
//Ein Dataset-Objekt erstellen.
DataSet ds = new DataSet();
//Datensatz mit den Tabellendatensätzen füllen.
da.Fill(ds, "Order Details");
//Eine Datentabelle in Bezug auf die Datensatztabelle erstellen.
DataTable dt = ds.Tables["Order Details"];
//WorkbookDesigner-Objekt erstellen.
WorkbookDesigner wd = new WorkbookDesigner();
//Öffnen Sie die Vorlagendatei (die intelligente Markierungen enthält).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
//Datentabelle als Datenquelle festlegen.
wd.SetDataSource(dt);
//Verarbeiten Sie die intelligenten Markierungen, um die Daten in die Arbeitsblätter einzufügen.
wd.Process(true);
//Speichern Sie die Excel-Datei.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Erstellen Sie ein Verbindungsobjekt, geben Sie die Anbieterinformationen an und legen Sie die Datenquelle fest.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Öffnen Sie das Verbindungsobjekt.
con.Open()
'Erstellen Sie ein Befehlsobjekt und geben Sie die SQL-Abfrage an.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Erstellen Sie ein Datenadapterobjekt.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Geben Sie den Befehl an.
da.SelectCommand = cmd
'Erstellen Sie ein Datensatzobjekt.
Dim ds As DataSet = New DataSet()
'Füllen Sie den Datensatz mit den Tabellendatensätzen.
da.Fill(ds, "Order Details")
'Erstellen Sie eine Datentabelle in Bezug auf die Datensatztabelle.
Dim dt As DataTable = ds.Tables("Order Details")
'WorkbookDesigner-Objekt erstellen.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Öffnen Sie die Vorlagendatei (die intelligente Markierungen enthält).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Legen Sie die Datentabelle als Datenquelle fest.
wd.SetDataSource(dt)
'Verarbeiten Sie die intelligenten Markierungen, um die Daten in die Arbeitsblätter einzufügen.
wd.Process(True)
'Speichern Sie die Excel-Datei.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Legt die Datenquelle eines DataTable-Objekts fest.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataTable | DataTable | DataTable-Objekt |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Legt die Datenquelle eines DataView-Objekts fest und bindet es an einen Datenquellennamen.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSourceName | String | Name der Datenquelle. |
| dataView | DataView | DataView-Objekt. |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Legt die Datenquelle eines DataView-Objekts fest.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataView | DataView | DataView-Objekt |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Legt die Datenquelle eines IDataReader-Objekts fest.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Kartenname der Datenquelle. |
| dataReader | IDataReader | IDataReader-Objekt |
| rowCount | Int32 | Die Anzahl der Datenzeilen. Wenn die intelligente Markierung nicht "noadd" enthält, müssen wir Zeilen nach der Zeilenanzahl für Leistungsprobleme und dynamische wiederholte Formeln einfügen. -1 bedeutet, dass der Parameter unbrauchbar ist. |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Legt die Datenbindung an eine Variable fest.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| variable | String | Mit Smart Marker erstellter Variablenname. |
| data | Object | Quelldaten. |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Legt die Datenquelle eines OleDbConnection-Objekts fest.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection-Objekt |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Legt die Datenquelle eines SqlConnection-Objekts fest.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection-Objekt |

### Siehe auch

* class [WorkbookDesigner](../../workbookdesigner)
* namensraum [Aspose.Cells](../../workbookdesigner)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
