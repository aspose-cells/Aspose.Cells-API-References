---
title: "Worksheet.ExportDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. يصدر البيانات في مجموعة Cells لورقة العمل إلى كائن DataTable محدد"
type: docs
url: /ar/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

يصدّر البيانات في مجموعة Cells لورقة عمل إلى كائن DataTable محدد.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| startColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| isVertical | منطقي | صحيح إذا كان الصف في التحكم يمثل صفًا في DataTable. خطأ إذا كان العمود في التحكم يمثل صفًا في DataTable. |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### ملاحظات

تسمح الطريقة أولاً بإنشاء كائن DataTable. ثم تصدر البيانات إلى كائن DataTable. إذا لم يتم تعيين dataTable بشكل صحيح، ستعيد الطريقة كائن DataTable جديد عن طريق استدعاء طريقة التحميل الزائدة 'Export(bool exportColumnName, bool isVertical)'.

### أمثلة

```csharp
[C#]

DataTable dataTable = new DataTable();
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"));
dataTable.Columns.Add("Column b");
dataTable.Columns.Add("Column c");
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"));
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"));
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"));
DataTable exportTable = gridDesktop.Worksheets[0].Export(dataTable,1,0,10,6,true);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim dataTable As DataTable =  New DataTable() 
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"))
dataTable.Columns.Add("Column b")
dataTable.Columns.Add("Column c")
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"))
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"))
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"))
Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(dataTable,1,0,10,6,True) 
DataGrid1.SetDataBinding(exportTable)
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

يصدّر البيانات في مجموعة Cells لورقة عمل إلى كائن DataTable جديد.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| startColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| exportColumnName | منطقي | يشير إلى ما إذا كانت البيانات في الصف الأول تُصدّر إلى اسم العمود في DataTable. |
| isVertical | منطقي | صحيح إذا كان الصف في التحكم يمثل صفًا في DataTable. خطأ إذا كان العمود في التحكم يمثل صفًا في DataTable. |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### أمثلة

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

تصدّر البيانات في مجموعة [`Cells`](../cells/) إلى كائن DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم استيرادها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| خيارات | GridExportTableOptions | جميع خيارات تصدير الجدول |

### قيمة الإرجاع

كائن DataTable المُصدّر.

### انظر أيضًا

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


