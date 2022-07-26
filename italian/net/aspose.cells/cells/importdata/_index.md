---
title: ImportData
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Importa i dati da aIDataReader oggetto.
type: docs
weight: 980
url: /it/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importa i dati da aIDataReader oggetto.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| reader | IDataReader | IlIDataReader oggetto che contiene dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |

### Valore di ritorno

Numero totale di righe importate.

### Guarda anche

* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importa i dati da aIDataReader oggetto.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| reader | IDataReader | IlIDataReader oggetto che contiene dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| options | ImportTableOptions | Le opzioni di importazione della tabella. |

### Valore di ritorno

Numero totale di righe importate.

### Guarda anche

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importa dati dalla tabella dati personalizzata.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | ICellsDataTable | La tabella dati personalizzata. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| options | ImportTableOptions | Le opzioni di importazione |

### Guarda anche

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importa dati dalla tabella dati personalizzata.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | DataTable | IlDataTable oggetto da importare. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| options | ImportTableOptions | Le opzioni di importazione |

### Valore di ritorno

Numero totale di righe importate.

### Esempi

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Importa dati
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

'Importa dati
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

'Esporta dati
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Guarda anche

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importa dati dalla visualizzazione dati.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataView | DataView | IlDataView oggetto da importare. |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| options | ImportTableOptions | Le opzioni di importazione |

### Valore di ritorno

Numero totale di righe importate.

### Guarda anche

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
