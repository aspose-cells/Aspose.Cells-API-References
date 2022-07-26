---
title: ImportData
second_title: Aspose.Cells for .NET API Referansı
description: Verileri birIDataReader nesne.
type: docs
weight: 980
url: /tr/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Verileri birIDataReader nesne.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| reader | IDataReader | buIDataReader veri içeren nesne. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Geri dönüş değeri

İçe aktarılan toplam satır sayısı.

### Ayrıca bakınız

* class [Cells](../../cells)
* ad alanı [Aspose.Cells](../../cells)
* toplantı [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Verileri birIDataReader nesne.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| reader | IDataReader | buIDataReader veri içeren nesne. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| options | ImportTableOptions | Tabloyu içe aktarma seçenekleri. |

### Geri dönüş değeri

İçe aktarılan toplam satır sayısı.

### Ayrıca bakınız

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* ad alanı [Aspose.Cells](../../cells)
* toplantı [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Özel veri tablosundan verileri içe aktarın.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| table | ICellsDataTable | Özel veri tablosu. |
| firstRow | Int32 | İlk satır dizini. |
| firstColumn | Int32 | İlk sütun dizini. |
| options | ImportTableOptions | içe aktarma seçenekleri |

### Ayrıca bakınız

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* ad alanı [Aspose.Cells](../../cells)
* toplantı [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Özel veri tablosundan verileri içe aktarın.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| table | DataTable | buDataTable içe aktarılacak nesne. |
| firstRow | Int32 | İlk satır dizini. |
| firstColumn | Int32 | İlk sütun dizini. |
| options | ImportTableOptions | içe aktarma seçenekleri |

### Geri dönüş değeri

İçe aktarılan toplam satır sayısı.

### Örnekler

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Verileri içe aktar
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

'Verileri içe aktar
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

'Verileri dışa aktar
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Ayrıca bakınız

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* ad alanı [Aspose.Cells](../../cells)
* toplantı [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Veri görünümünden verileri içe aktarın.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataView | DataView | buDataView içe aktarılacak nesne. |
| firstRow | Int32 | İlk satır dizini. |
| firstColumn | Int32 | İlk sütun dizini. |
| options | ImportTableOptions | içe aktarma seçenekleri |

### Geri dönüş değeri

İçe aktarılan toplam satır sayısı.

### Ayrıca bakınız

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* ad alanı [Aspose.Cells](../../cells)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
