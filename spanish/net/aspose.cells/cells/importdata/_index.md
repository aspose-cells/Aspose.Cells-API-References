---
title: ImportData
second_title: Referencia de API de Aspose.Cells para .NET
description: Importa datos de unIDataReader objeto.
type: docs
weight: 980
url: /es/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importa datos de unIDataReader objeto.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| reader | IDataReader | losIDataReader objeto que contiene datos. |
| firstRow | Int32 | El número de fila de la primera celda a importar. |
| firstColumn | Int32 | El número de columna de la primera celda a importar. |

### Valor_devuelto

Número total de filas importadas.

### Ver también

* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importa datos de unIDataReader objeto.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| reader | IDataReader | losIDataReader objeto que contiene datos. |
| firstRow | Int32 | El número de fila de la primera celda a importar. |
| firstColumn | Int32 | El número de columna de la primera celda a importar. |
| options | ImportTableOptions | Las opciones de importar tabla. |

### Valor_devuelto

Número total de filas importadas.

### Ver también

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importar datos de la tabla de datos personalizados.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| table | ICellsDataTable | La tabla de datos personalizados. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de la primera columna. |
| options | ImportTableOptions | Las opciones de importación |

### Ver también

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importar datos de la tabla de datos personalizados.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| table | DataTable | losDataTable objeto a importar. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de la primera columna. |
| options | ImportTableOptions | Las opciones de importación |

### Valor_devuelto

Número total de filas importadas.

### Ejemplos

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Datos de importacion
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

'Datos de importacion
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

'Exportar datos
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Ver también

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importar datos desde la vista de datos.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| dataView | DataView | losDataView objeto a importar. |
| firstRow | Int32 | Índice de la primera fila. |
| firstColumn | Int32 | Índice de la primera columna. |
| options | ImportTableOptions | Las opciones de importación |

### Valor_devuelto

Número total de filas importadas.

### Ver también

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
