---
title: SetDataSource
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Imposta lorigine dati di aICellsDataTableaspose.cells/icellsdatatable oggetto.
type: docs
weight: 120
url: /it/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Imposta l'origine dati di a[`ICellsDataTable`](../../icellsdatatable) oggetto.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSource | String | Il nome dell'origine dati. |
| cellsDataTable | ICellsDataTable | tabella dati. |

### Guarda anche

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Imposta l'origine dati di un oggetto DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSet | DataSet | oggetto DataSet |

### Esempi

```csharp

[C#]

//Crea un oggetto di connessione, specifica le informazioni sul provider e imposta l'origine dati.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Apri l'oggetto connessione.
con.Open();
//Crea un oggetto comando e specifica la query SQL.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Crea un oggetto adattatore dati.
OleDbDataAdapter da = new OleDbDataAdapter();
//Specifica il comando.
da.SelectCommand = cmd;
//Crea un oggetto set di dati.
DataSet ds = new DataSet();
//Riempi il set di dati con i record della tabella.
da.Fill(ds, "Order Details");
//Crea un datatable rispetto alla tabella del set di dati.
DataTable dt = ds.Tables["Order Details"];
//Crea oggetto WorkbookDesigner.
WorkbookDesigner wd = new WorkbookDesigner();
//Apri il file modello (che contiene marcatori intelligenti).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
//Imposta il datatable come origine dati.
wd.SetDataSource(dt);
//Elabora gli indicatori intelligenti per inserire i dati nei fogli di lavoro.
wd.Process(true);
//Salva il file excel.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Crea un oggetto di connessione, specifica le informazioni sul provider e imposta l'origine dati.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Aprire l'oggetto di connessione.
con.Open()
'Creare un oggetto comando e specificare la query SQL.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Creare un oggetto adattatore dati.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Specificare il comando.
da.SelectCommand = cmd
'Crea un oggetto set di dati.
Dim ds As DataSet = New DataSet()
'Riempi il set di dati con i record della tabella.
da.Fill(ds, "Order Details")
'Creare una tabella dati rispetto alla tabella del set di dati.
Dim dt As DataTable = ds.Tables("Order Details")
'Crea oggetto WorkbookDesigner.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Apri il file modello (che contiene marcatori intelligenti).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Imposta il datatable come origine dati.
wd.SetDataSource(dt)
'Elabora i marcatori intelligenti per inserire i dati nei fogli di lavoro.
wd.Process(True)
'Salva il file excel.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Imposta l'origine dati di un oggetto DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataTable | DataTable | Oggetto DataTable |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Imposta l'origine dati di un oggetto DataView e lo associa a un nome di origine dati.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSourceName | String | Nome origine dati. |
| dataView | DataView | Oggetto DataView. |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Imposta l'origine dati di un oggetto DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataView | DataView | Oggetto DataView |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Imposta l'origine dati di un oggetto IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della mappa dell'origine dati. |
| dataReader | IDataReader | Oggetto IDataReader |
| rowCount | Int32 | Il numero delle righe di dati. Se l'indicatore intelligente non contiene "noadd", dobbiamo inserire le righe in base al conteggio delle righe per problemi di prestazioni e formule ripetute dinamiche. -1 significa che il parametro è inutile. |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Imposta il data binding su una variabile.

```csharp
public void SetDataSource(string variable, object data)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| variable | String | Nome della variabile creato utilizzando un marcatore intelligente. |
| data | Object | Dati di origine. |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Imposta l'origine dati di un oggetto OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | OleDbConnection | Oggetto OleDbConnection |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Imposta l'origine dati di un oggetto SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connection | SqlConnection | Oggetto SQLConnection |

### Guarda anche

* class [WorkbookDesigner](../../workbookdesigner)
* spazio dei nomi [Aspose.Cells](../../workbookdesigner)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
