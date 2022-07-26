---
title: SetDataSource
second_title: Aspose.Cells لمرجع .NET API
description: يحدد مصدر بيانات ملفICellsDataTableaspose.cells/icellsdatatable الكائن .
type: docs
weight: 120
url: /ar/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

يحدد مصدر بيانات ملف[`ICellsDataTable`](../../icellsdatatable) الكائن .

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataSource | String | اسم مصدر البيانات. |
| cellsDataTable | ICellsDataTable | جدول البيانات. |

### أنظر أيضا

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

تعيين مصدر البيانات لكائن DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataSet | DataSet | كائن DataSet |

### أمثلة

```csharp

[C#]

// إنشاء كائن اتصال ، وتحديد معلومات الموفر وتعيين مصدر البيانات.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
// افتح كائن الاتصال.
con.Open();
// إنشاء كائن أمر وتحديد استعلام SQL.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
// إنشاء كائن محول البيانات.
OleDbDataAdapter da = new OleDbDataAdapter();
// حدد الأمر.
da.SelectCommand = cmd;
// إنشاء كائن مجموعة بيانات.
DataSet ds = new DataSet();
// املأ مجموعة البيانات بسجلات الجدول.
da.Fill(ds, "Order Details");
// إنشاء جدول بيانات فيما يتعلق بجدول مجموعة البيانات.
DataTable dt = ds.Tables["Order Details"];
// إنشاء كائن WorkbookDesigner.
WorkbookDesigner wd = new WorkbookDesigner();
// افتح ملف القالب (الذي يحتوي على علامات ذكية).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
// قم بتعيين جدول البيانات كمصدر للبيانات.
wd.SetDataSource(dt);
// معالجة العلامات الذكية لملء البيانات في أوراق العمل.
wd.Process(true);
// احفظ ملف Excel.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'قم بإنشاء كائن اتصال ، وحدد معلومات الموفر وقم بتعيين مصدر البيانات.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'افتح كائن الاتصال.
con.Open()
'قم بإنشاء كائن أمر وحدد استعلام SQL.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'إنشاء كائن محول البيانات.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'حدد الأمر.
da.SelectCommand = cmd
'قم بإنشاء كائن مجموعة بيانات.
Dim ds As DataSet = New DataSet()
'املأ مجموعة البيانات بسجلات الجدول.
da.Fill(ds, "Order Details")
'قم بإنشاء جدول بيانات فيما يتعلق بجدول مجموعة البيانات.
Dim dt As DataTable = ds.Tables("Order Details")
'إنشاء كائن WorkbookDesigner.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'افتح ملف القالب (الذي يحتوي على علامات ذكية).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'قم بتعيين جدول البيانات كمصدر للبيانات.
wd.SetDataSource(dt)
'قم بمعالجة العلامات الذكية لملء البيانات في أوراق العمل.
wd.Process(True)
'احفظ ملف اكسل.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

تعيين مصدر البيانات لكائن DataTable .

```csharp
public void SetDataSource(DataTable dataTable)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataTable | DataTable | كائن DataTable |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

تعيين مصدر البيانات لكائن DataView وربطه باسم مصدر البيانات.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataSourceName | String | اسم مصدر البيانات. |
| dataView | DataView | كائن DataView. |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

تعيين مصدر البيانات لكائن DataView .

```csharp
public void SetDataSource(DataView dataView)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dataView | DataView | كائن DataView |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

تعيين مصدر البيانات لكائن IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم خريطة مصدر البيانات. |
| dataReader | IDataReader | كائن IDataReader |
| rowCount | Int32 | عدد صفوف البيانات. إذا كانت العلامة الذكية لا تحتوي على "noadd" ، يتعين علينا إدراج صفوف من خلال عدد الصفوف لمشكلة الأداء والصيغ المكررة الديناميكية. -1 يعني أن المعلمة عديمة الفائدة. |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

يعين ربط البيانات بمتغير .

```csharp
public void SetDataSource(string variable, object data)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| variable | String | تم إنشاء اسم متغير باستخدام علامة ذكية. |
| data | Object | مصدر معلومات. |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

تعيين مصدر البيانات لكائن OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | OleDbConnection | كائن OleDbConnection |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

يعين مصدر البيانات لكائن SqlConnection .

```csharp
public void SetDataSource(SqlConnection connection)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| connection | SqlConnection | كائن SqlConnection |

### أنظر أيضا

* class [WorkbookDesigner](../../workbookdesigner)
* مساحة الاسم [Aspose.Cells](../../workbookdesigner)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
