---
title: "PivotField.Top10AutoShow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Bu pivot alanı için Top10 AutoShow ayarlarını yapılandırır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Bu pivot alanı için Top10 AutoShow ayarlarını yapılandırır.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoShow | Boolean | AutoShow'u etkinleştirmek için true; devre dışı bırakmak için false. |
| isTop | Boolean | True ise üst öğeleri gösterir; false ise alt öğeleri gösterir. |
| sayım | Int32 | Gösterilecek üst/alt öğe sayısı. |
| rankBy | Int32 | Sıralama için kullanılan veri alanının dizini. PivotItem'ın kendi değerlerine göre sıralamak için -1 kullanın. |

### Açıklamalar

Bu yöntem, [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/) yapılandırır.

XLS ikili formatı: AutoShow (Top10) yerel ve tek desteklenen seçenektir.

XLSX (OpenXML): Temel dosya formatı Top10 AutoShow'u destekler, ancak Excel 2007 ve sonraki sürümlerin kullanıcı arayüzü bunu yalnızca Top10 filtresi aracılığıyla gösterir. XLS uyumluluğu gerekmezse, bunun yerine Top10 filtresinin kullanılması önerilir.

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


