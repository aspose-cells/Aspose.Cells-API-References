---
title: "Sınıf PivotTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.PivotTables sınıfı. Tüm PivotTable nesnelerinin bir koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Tüm [`PivotTable`](../pivottable/) nesnelerinin bir koleksiyonunu temsil eder

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | PivotTables örneğinde bulunan öğe sayısını alır |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | PivotTables erişiminin senkronize (iş parçacığı güvenli) olup olmadığını gösteren bir değer alır. |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | İndeks ile bir PivotTable nesnesi alır. (2 indeksleyici) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Belirtilen nesne için üst nesneyi alır. Salt okunur. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | PivotTables erişimini senkronize etmek için kullanılabilecek bir nesne alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Belirtilen PivotCache'ten yeni bir çalışma sayfasına bir PivotTable nesnesi ekler |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Belirtilen PivotCache'ten yeni bir çalışma sayfasına bir PivotTable nesnesi ekler |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Belirtilen PivotCache'ten belirtilen çalışma sayfasına bir PivotTable nesnesi ekler |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Belirtilen PivotCache'ten belirtilen çalışma sayfasına bir PivotTable nesnesi ekler |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Kontrol içindeki tüm PivotTable nesnelerini ve tüm PivotCache nesnelerini kaldırır. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | pivottable adı tableName mevcutsa true döndürür. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | PivotTable'ın tamamını uyumlu tek boyutlu bir diziye kopyalar, hedef dizinin belirtilen indeksinden başlayarak |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | PivotTable'lar için bir IEnumerator döndürür. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | Veri kaynağını PivotTable raporuna yeniden bağlar. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | Veri kaynağını tüm PivotTable raporlarına yeniden bağlar. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Belirtilen PivotTable nesnesini PivotTable'lardan ve ilgili PivotCache'ten kaldırır, eğer başka bir PivotTable tarafından kullanılmıyorsa |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Belirtilen PivotTable nesnesini PivotTable'lardan ve ilgili PivotCache'ten kaldırır, eğer başka bir PivotTable tarafından kullanılmıyorsa |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Lütfen bunun yerine GridPivotTableCollection kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp

 [C#]

 //Çalışma sayfası "Sheet1"'de veri olduğu varsayımıyla, buna dayalı bir PivotTable raporu oluşturur.
 WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
 Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
 sourceRange.StartRow = 0;
 sourceRange.StartColumn = 0;
 sourceRange.EndRow = 10;
 sourceRange.EndColumn = 5;

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);

 PivotTable table = cache.CreatePivotTable();

 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
 table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;

 table.PivotFields[3].Function = PivotFieldFunction.Count;
 table.PivotFields[5].Function = PivotFieldFunction.Sum;

 table.DataBind();

 //DataView veya DataTable'dan bir PivotTable raporu oluşturur.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Or PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
 PivotTable table = cache.CreatePivotTable();
 table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.DataBind();


 [VB]


 'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
 Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
 Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
 sourceRange.StartRow = 0
 sourceRange.StartColumn = 0
 sourceRange.EndRow = 10
 sourceRange.EndColumn = 5

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)

 Dim table As PivotTable =  cache.CreatePivotTable()

 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
 table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField

 table.PivotFields(3).Function = PivotFieldFunction.Count
 table.PivotFields(5).Function = PivotFieldFunction.Sum

 table.DataBind()

 'Creates a PivotTable report from DataView or DataTable.

 Dim dataView As DataView ' Or Dim dataTable As DataTable
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
 'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
 Dim table As PivotTable =  cache.CreatePivotTable()
 table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.DataBind()

```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


