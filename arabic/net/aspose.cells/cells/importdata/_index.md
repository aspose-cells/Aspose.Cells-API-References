---
title: ImportData
second_title: Aspose.Cells لمرجع .NET API
description: يستورد البيانات من ملفIDataReader الكائن .
type: docs
weight: 980
url: /ar/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

يستورد البيانات من ملفIDataReader الكائن .

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| reader | IDataReader | الIDataReader الكائن الذي يحتوي على بيانات. |
| firstRow | Int32 | رقم صف الخلية الأولى المطلوب الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### قيمة الإرجاع

إجمالي عدد الصفوف التي تم استيرادها.

### أنظر أيضا

* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

يستورد البيانات من ملفIDataReader الكائن .

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| reader | IDataReader | الIDataReader الكائن الذي يحتوي على بيانات. |
| firstRow | Int32 | رقم صف الخلية الأولى المطلوب الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| options | ImportTableOptions | خيارات استيراد الجدول. |

### قيمة الإرجاع

إجمالي عدد الصفوف التي تم استيرادها.

### أنظر أيضا

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

استيراد البيانات من جدول البيانات المخصصة .

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| table | ICellsDataTable | جدول البيانات المخصصة. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| options | ImportTableOptions | خيارات الاستيراد |

### أنظر أيضا

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

استيراد البيانات من جدول البيانات المخصصة .

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| table | DataTable | الDataTable كائن سيتم استيراده. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| options | ImportTableOptions | خيارات الاستيراد |

### قيمة الإرجاع

إجمالي عدد الصفوف التي تم استيرادها.

### أمثلة

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//بيانات الاستيراد
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

'بيانات الاستيراد
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

'تصدير البيانات
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### أنظر أيضا

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

استيراد البيانات من عرض البيانات .

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataView | DataView | الDataView كائن سيتم استيراده. |
| firstRow | Int32 | فهرس الصف الأول. |
| firstColumn | Int32 | فهرس العمود الأول. |
| options | ImportTableOptions | خيارات الاستيراد |

### قيمة الإرجاع

إجمالي عدد الصفوف التي تم استيرادها.

### أنظر أيضا

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
