---
title: "Worksheet.ExportDataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bir Worksheet'in Cells koleksiyonundaki verileri belirtilen bir DataTable nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Worksheet'in Cells koleksiyonundaki verileri belirtilen bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| isVertical | Boolean | Kontrol içindeki bir satır DataTable'da bir satırı temsil ediyorsa doğru. Kontrol içindeki bir sütun DataTable'da bir satırı temsil ediyorsa yanlış. |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Açıklamalar

Yöntem, önce bir DataTable nesnesi oluşturulmasına izin verir. Ardından verileri DataTable nesnesine dışa aktarır. Eğer dataTable geçerli şekilde ayarlanmamışsa, yöntem 'Export(bool exportColumnName, bool isVertical)' aşırı yükleme metodunu çağırarak yeni bir DataTable nesnesi döndürecektir.

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

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Worksheet'in Cells koleksiyonundaki verileri yeni bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| exportColumnName | Boolean | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını belirtir. |
| isVertical | Boolean | Kontrol içindeki bir satır DataTable'da bir satırı temsil ediyorsa doğru. Kontrol içindeki bir sütun DataTable'da bir satırı temsil ediyorsa yanlış. |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Örnekler

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Verileri [`Cells`](../cells/) koleksiyonundaki bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |
| seçenekler | GridExportTableOptions | Tüm dışa aktarma tablo seçenekleri |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Ayrıca Bakınız

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


