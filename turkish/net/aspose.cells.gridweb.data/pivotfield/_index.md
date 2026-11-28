---
title: "PivotField sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.PivotField sınıfı. PivotTable raporunda bir alanı temsil eder. PivotField nesnesi PivotFields koleksiyonunun bir üyesidir.  NOT Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen GridPivotField kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler."
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

PivotTable raporunda bir alanı temsil eder. PivotField nesnesi [`PivotFields`](../pivotfields/) koleksiyonunun bir üyesidir.  NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen GridPivotField kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Rapor içinde gösterilen pivot alanı etiketi metni. Varsayılan olarak adı gösterir. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Belirtilen alanın verisini alır. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | PivotTable alanını (yalnızca veri alanları) özetlemek için kullanılan işlevi temsil eder. Varsayılan işlev Count'tur. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Adı alır. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Belirtilen PivotTable raporundaki alanın konumunu temsil eder. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Alanın (ilk, ikinci, üçüncü vb.) konumunu, yönlendirmesindeki (Satırlar, Sütunlar, Sayfalar) tüm alanlar arasında temsil eder. Pivottable.DataBind çağrıldıktan sonra get metodunu çağırmalısınız. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Belirtilen PivotTable alanını sıralamak için kullanılan sıralamayı temsil eder. |

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


