---
title: SetDataSource
second_title: Aspose.Cells for .NET API Referansı
description: Bir veri kaynağını ayarlarICellsDataTableaspose.cells/icellsdatatable nesne.
type: docs
weight: 120
url: /tr/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Bir veri kaynağını ayarlar[`ICellsDataTable`](../../icellsdatatable) nesne.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataSource | String | Veri kaynağının adı. |
| cellsDataTable | ICellsDataTable | veri tablosu. |

### Ayrıca bakınız

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Bir DataSet nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataSet | DataSet | Veri Kümesi nesnesi |

### Örnekler

```csharp

[C#]

//Bir bağlantı nesnesi oluşturun, sağlayıcı bilgilerini belirtin ve veri kaynağını ayarlayın.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Bağlantı nesnesini açın.
con.Open();
//Bir komut nesnesi oluşturun ve SQL sorgusunu belirtin.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Bir veri bağdaştırıcı nesnesi oluşturun.
OleDbDataAdapter da = new OleDbDataAdapter();
// Komutu belirtin.
da.SelectCommand = cmd;
// Bir veri kümesi nesnesi oluşturun.
DataSet ds = new DataSet();
//Veri kümesini tablo kayıtlarıyla doldurun.
da.Fill(ds, "Order Details");
//Veri kümesi tablosuna göre bir veri tablosu oluşturun.
DataTable dt = ds.Tables["Order Details"];
//WorkbookDesigner nesnesi oluştur.
WorkbookDesigner wd = new WorkbookDesigner();
//Şablon dosyasını açın (akıllı işaretçileri içerir).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
// Veri tablosunu veri kaynağı olarak ayarlayın.
wd.SetDataSource(dt);
// Verileri çalışma sayfalarına doldurmak için akıllı işaretçileri işleyin.
wd.Process(true);
//Excel dosyasını kaydedin.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Bir bağlantı nesnesi oluşturun, sağlayıcı bilgilerini belirtin ve veri kaynağını ayarlayın.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Bağlantı nesnesini açın.
con.Open()
'Bir komut nesnesi oluşturun ve SQL sorgusunu belirtin.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Bir veri bağdaştırıcı nesnesi oluşturun.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Komutu belirtin.
da.SelectCommand = cmd
'Bir veri kümesi nesnesi oluşturun.
Dim ds As DataSet = New DataSet()
'Veri kümesini tablo kayıtlarıyla doldurun.
da.Fill(ds, "Order Details")
'Veri kümesi tablosuna göre bir veri tablosu oluşturun.
Dim dt As DataTable = ds.Tables("Order Details")
'WorkbookDesigner nesnesi oluşturun.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'(Akıllı işaretler içeren) şablon dosyasını açın.
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Veri tablosunu veri kaynağı olarak ayarlayın.
wd.SetDataSource(dt)
'Verileri çalışma sayfalarına doldurmak için akıllı işaretleri işleyin.
wd.Process(True)
'Excel dosyasını kaydedin.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

DataTable nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataTable | DataTable | DataTable nesnesi |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Bir DataView nesnesinin veri kaynağını ayarlar ve onu bir veri kaynağı adına bağlar.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataSourceName | String | Veri kaynağı adı. |
| dataView | DataView | DataView nesnesi. |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Bir DataView nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataView dataView)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataView | DataView | DataView nesnesi |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Bir IDataReader nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| name | String | Veri kaynağı eşleme adı. |
| dataReader | IDataReader | IDataReader nesnesi |
| rowCount | Int32 | Veri satırlarının sayısı. Akıllı işaretçi "noadd" içermiyorsa, performans sorunu ve dinamik tekrarlanan formüller için satır sayısına göre satır eklememiz gerekir. -1, parametrenin işe yaramaz olduğu anlamına gelir. |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Bir değişkene veri bağlamayı ayarlar.

```csharp
public void SetDataSource(string variable, object data)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| variable | String | Akıllı işaretleyici kullanılarak oluşturulan değişken adı. |
| data | Object | Kaynak verileri. |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Bir OleDbConnection nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection nesnesi |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Bir SqlConnection nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection nesnesi |

### Ayrıca bakınız

* class [WorkbookDesigner](../../workbookdesigner)
* ad alanı [Aspose.Cells](../../workbookdesigner)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
