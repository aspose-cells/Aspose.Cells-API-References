---
title: "Sınıf PivotFields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.PivotFields sınıfı. PivotTable raporundaki tüm PivotField nesnelerinin bir koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Bir PivotTable raporundaki tüm [`PivotField`](../pivotfield/) nesnelerinin koleksiyonunu temsil eder.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | PivotFields örneğinde bulunan öğe sayısını alır. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | PivotFields erişiminin senkronize (iş parçacığı güvenli) olup olmadığını gösteren bir değeri alır. |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | İndeksle bir PivotField alır. (2 indeksleyici) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Belirtilen nesne için üst nesneyi alır. Salt okunur. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | PivotFields erişimini senkronize etmek için kullanılabilecek bir nesneyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Tam PivotField'ı, hedef dizinin belirtilen indeksinden başlayarak uyumlu tek boyutlu bir diziye kopyalar |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | PivotFields için bir IEnumerator döndürür. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Belirtilen PivotField'ın indeksini alır. |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine GridPivotFieldCollection kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp

 [C#]

 //PivotTable[0] için PivotFields alır
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //PivotFields konumunu ayarlar
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Veri alanının işlevini ayarlar
 field3.Function = PivotFieldFunction.Sum;

 //Satır alanlarının sırasını değiştirir
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


