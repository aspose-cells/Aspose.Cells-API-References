---
title: Cells.ImportDataTable
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataTable object into a worksheet
type: docs
url: /net/aspose.cells/cells/importdatatable/
---
## ImportDataTable(DataTable, bool, string) {#importdatatable_7}

Imports a DataTable object into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, string startCell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. |
| startCell | String | The name of start cell to insert the DataTable, such as "A2". |

### Return Value

Total number of rows imported

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, bool, bool) {#importdatatable_2}

Imports a DataTable object into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, bool insertRows, bool convertStringToNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import. |
| firstColumn | Int32 | The column number of the first cell to import. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| convertStringToNumber | Boolean | Indicates if this method will try to convert string to number. |

### Return Value

Total number of rows imported

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int) {#importdatatable}

Imports a DataTable object into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import. |
| firstColumn | Int32 | The column number of the first cell to import. |

### Return Value

Total number of rows imported

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, bool) {#importdatatable_1}

Imports a DataTable object into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, bool insertRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import. |
| firstColumn | Int32 | The column number of the first cell to import. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |

### Return Value

Total number of rows imported

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, int, int) {#importdatatable_3}

Imports a DataTable into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |

### Return Value

Total number of rows imported

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp

[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

DataTable dt = new DataTable("Employee");
dt.Columns.Add("Employee_ID",typeof(Int32));
dt.Columns.Add("Employee_Name",typeof(string));
dt.Columns.Add("Gender",typeof(string));
DataRow dr = dt.NewRow();
dr[0] = 1;
dr[1] = "John Smith";
dr[2] = "Male";
dt.Rows.Add(dr);
dr = dt.NewRow();
dr[0] = 2;
dr[1] = "Mary Miller";
dr[2] = "Female";
dt.Rows.Add(dr);
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
cells.ImportData(dt, 12, 12, options);

[Visual Basic]
Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells
Dim dt As DataTable =  New DataTable("Employee") 
dt.Columns.Add("Employee_ID",Type.GetType(Int32))
dt.Columns.Add("Employee_Name",Type.GetType(String))
dt.Columns.Add("Gender",Type.GetType(String))
Dim dr As DataRow =  dt.NewRow() 
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
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, int, int, bool, string) {#importdatatable_5}

Imports a DataTable into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, int rowNumber, int columnNumber, bool insertRows, string dateFormatString)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| columnNumber | Int32 | Number of columns to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | String | Date format string for cells. |

### Return Value

Total number of rows imported.

### Remarks

This method automatically format date time values. However, if the DateTable is very huge, this method may slow down the program. In this case, you'd better format the cell manually.

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, int, int, bool, string, bool) {#importdatatable_6}

Imports a DataTable into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, int rowNumber, int columnNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| columnNumber | Int32 | Number of columns to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | String | Date format string for cells. |
| convertStringToNumber | Boolean | Indicates if this method will try to convert string to number. |

### Return Value

Total number of rows imported.

### Remarks

This method automatically format date time values. However, if the DateTable is very huge, this method may slow down the program. In this case, you'd better format the cell manually.

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataTable(DataTable, bool, int, int, int, int, bool) {#importdatatable_4}

Imports a DataTable into a worksheet.

```csharp
[Obsolete("Use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ImportDataTable(DataTable dataTable, bool isFieldNameShown, int firstRow, 
    int firstColumn, int rowNumber, int columnNumber, bool insertRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | The DataTable object to be imported. |
| isFieldNameShown | Boolean | Indicates whether the field name of the datatable will be imported to the first row. Default is true. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| columnNumber | Int32 | Number of columns to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |

### Return Value

Total number of rows imported.

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(DataTable,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


