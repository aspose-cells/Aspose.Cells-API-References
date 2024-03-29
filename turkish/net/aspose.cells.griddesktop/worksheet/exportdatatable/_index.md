---
title: ExportDataTable
second_title: Aspose.Cells for .NET API Referansı
description: Bir Çalışma Sayfasının Hücreler koleksiyonundaki verileri belirtilen bir DataTable nesnesine verir.
type: docs
weight: 650
url: /tr/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(DataTable, int, int, int, int, bool) {#exportdatatable_1}

Bir Çalışma Sayfasının Hücreler koleksiyonundaki verileri belirtilen bir DataTable nesnesine verir.

```csharp
public DataTable ExportDataTable(DataTable dataTable, int startRow, int startColumn, int rows, 
    int columns, bool isVertical)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| dataTable | DataTable | Verileri dışa aktaran DataTable nesnesi. |
| startRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| rows | Int32 | İçe aktarılacak satır sayısı. |
| columns | Int32 | İçe aktarılacak sütun sayısı. |
| isVertical | Boolean | Denetimdeki bir satır DataTable'daki bir satırı temsil ediyorsa doğrudur. Denetimdeki bir sütun DataTable'daki bir satırı temsil ediyorsa False. |

### Geri dönüş değeri

Dışa aktarılan DataTable nesnesi.

### Notlar

Yöntem, önce bir DataTable nesnesi oluşturmaya izin verir. Ardından verileri DataTable nesnesine aktarır. dataTable geçerli ayarlanmazsa, yöntem 'Export(bool exportColumnName, bool isVertical)' aşırı yükleme yöntemini çağırarak yeni bir DataTable nesnesi döndürür.

### Örnekler

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

### Ayrıca bakınız

* class [Worksheet](../../worksheet)
* ad alanı [Aspose.Cells.GridDesktop](../../worksheet)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable}

Çalışma Sayfasının Hücreler koleksiyonundaki verileri yeni bir DataTable nesnesine aktarır.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| startRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| rows | Int32 | İçe aktarılacak satır sayısı. |
| columns | Int32 | İçe aktarılacak sütun sayısı. |
| exportColumnName | Boolean | İlk satırdaki verilerin DataTable sütun adına dışa aktarılıp aktarılmadığını gösterir. |
| isVertical | Boolean | Denetimdeki bir satır DataTable'daki bir satırı temsil ediyorsa doğrudur. Denetimdeki bir sütun DataTable'daki bir satırı temsil ediyorsa False. |

### Geri dönüş değeri

Dışa aktarılan DataTable nesnesi.

### Örnekler

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Ayrıca bakınız

* class [Worksheet](../../worksheet)
* ad alanı [Aspose.Cells.GridDesktop](../../worksheet)
* toplantı [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
