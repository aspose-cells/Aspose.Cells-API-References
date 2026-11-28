---
title: "Sınıf PivotCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.PivotCache sınıfı. PivotTable raporu için bellek önbelleğini temsil eder. PivotCache nesnesi, PivotCaches koleksiyonunun bir üyesidir"
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

PivotTable raporu için bellek önbelleğini temsil eder. PivotCache nesnesi, [`PivotCaches`](../pivotcaches/) koleksiyonunun bir üyesidir.

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | PivotTable raporu için System.Data.DataTable veri kaynağını döndürür. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | PivotTable raporu için System.Data.DataView veri kaynağını döndürür. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Bu nesnenin ebeveyn içindeki indeksini döndürür |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | PivotCache.Re adını döndürür |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Belirtilen nesne için üst nesneyi döndürür (PivotCache'in kapsayıcısı). Salt okunur. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | SourceSheet ile kullanılan veri kaynağının aralığını döndürür. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | PivotTable raporu için WebWorksheet veri kaynağını döndürür. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Kaynak verinin tipini temsil eder |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Yeni bir Sayfaya PivotTable raporu oluşturur. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Yeni bir Sayfaya PivotTable raporu oluşturur. pivotTable nesnesinin adı |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | targetSheet'e PivotTable raporu oluşturur. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | targetSheet'e PivotTable raporu oluşturur. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | İki Object örneğinin eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Belirli bir tip için bir hash işlevi olarak hizmet verir, hash tabloları gibi hash algoritmaları ve veri yapılarında kullanılmaya uygundur. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Kaynak verileri sıfırlar |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Kaynak verileri sıfırlar |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Kaynak verileri sıfırlar |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Geçerli Object'i temsil eden bir String döndürür |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Lütfen bunun yerine GridPivotTable kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

PivotCache metodunu kullanarak bir PivotTable raporu için PivotCache nesnesi döndürür (her rapor yalnızca bir önbelleğe sahiptir). PivotCache'in kaynak verileri WebWorksheet, DataTable vb. kaynaklardan gelir.

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


