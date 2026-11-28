---
title: "Sınıf PivotCaches"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.PivotCaches sınıf. Bir çalışma kitabındaki PivotTable raporlarından gelen bellek önbelleklerinin koleksiyonunu temsil eder. Her bellek önbelleği bir PivotCache nesnesiyle temsil edilir."
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Bir çalışma kitabındaki PivotTable raporlarından gelen bellek önbelleklerinin koleksiyonunu temsil eder. Her bellek önbelleği bir [`PivotCache`](../pivotcache/) nesnesiyle temsil edilir.

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | PivotCaches örneğinde bulunan eleman sayısını alır |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | PivotCaches erişiminin senkronize (iş parçacığı güvenli) olup olmadığını gösteren bir değer alır. |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | İndeksle PivotCache nesnesi alır. (2 indeksleyici) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Belirtilen nesne için üst nesneyi alır. Salt okunur. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | PivotCaches erişimini senkronize etmek için kullanılabilecek bir nesne alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | DataTable'dan bir PivotCache ekler. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | DataView'dan bir PivotCache ekler. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Belirtilen adı kullanarak DataTable'dan bir PivotCahe ekler. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Belirtilen adı kullanarak DataView'den bir PivotCahe ekler. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Sayfadan bir PivotCache ekler |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Belirtilen adı kullanarak sayfadan bir PivotCache ekler. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Kontrol içindeki tüm PivotCache nesnelerini ve tüm PivotTable nesnelerini kaldırır. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Tüm PivotCache'i uyumlu tek boyutlu bir Array'ye, hedef dizinin belirtilen indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | PivotCaches için bir IEnumerator döndürür. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Koleksiyondaki belirtilen PivotCache'in dizinini döndürür. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | pivotCache'i veri kaynağı olarak kullanarak PivotCaches'ten belirtilen PivotCache nesnesini ve ilgili PivotTable'ı kaldırır. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | pivotCache'i veri kaynağı olarak kullanarak PivotCaches'ten belirtilen PivotCache nesnesini ve ilgili PivotTable'ı kaldırır. |

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


