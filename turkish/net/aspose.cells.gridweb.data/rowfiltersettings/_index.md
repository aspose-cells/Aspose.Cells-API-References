---
title: "Sınıf RowFilterSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings class. RowFilter için özet açıklama"
type: docs
url: /tr/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

RowFilter için özet açıklama.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | Filtre kriter dizesi. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Otomatik filtrelemeyi etkinleştirir. HeaderRow, kullanıcının filtrelenecek sütunun değerini seçebilmesi için açılır düğmeler gösterir. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Filtre aralığının son satır numarası. Bu değer -1 olarak ayarlanırsa, sayfanın son satır numarası kullanılır. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Filtre açılır düğmelerini gösterecek başlık satır numarası. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Filtre aralığının başlangıç satır numarası. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Otomatik filtre ayarlarından kriter dizesi oluşturur. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Tüm filtre ayarlarını temizler ve tüm satırları gösterir. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Özel bir filtre belirtir. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Satırları kriter dizesi kullanarak filtreler. |

### Açıklamalar

NOT: Bu sınıf artık eski. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacak. Otomatik filtre / özel filtre ayarları için GridWorksheet AddAutoFilter/FilterString kullanabilirsiniz. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


