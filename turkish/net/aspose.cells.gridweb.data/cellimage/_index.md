---
title: "Sınıf CellImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.CellImage sınıfı. Görüntü src'siyle bir hiperlinki temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Görsel src'li bir hyperlink'i temsil eder.

```csharp
public class CellImage : Hyperlink
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Hiperlinkin eylem türünü alır veya ayarlar. ActionTpye.UrlLink veya ActionType.CellCommand olabilir. UrlLink türü, hiperlinkin bir web sayfasına veya e-posta alıcısına bağlantı olduğu anlamına gelir. Örneğin: "http://www.aspose.com" veya "mailto:admin@aspose.com". CellCommand türü, hiperlinkin bir CellCommand olayı tetikleyeceği ve bu olayı işleyebileceğiniz anlamına gelir.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Hiperlinkin kapsamını alır.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Cell Command adını alır veya ayarlar.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Kullanıcı bu CellCommand hiperlinkine tıkladığında istemci tarayıcısındaki kullanıcı girdisinin atılıp atılmayacağını gösterir. "Geri alma" eylemi olarak kullanılabilir.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Hiperlinkin görüntü URL'sini alır veya ayarlar. Null veya boş string olarak ayarlanırsa, hiperlink yalnızca metnini gösterir.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Hiperlinkin görüntülenen metnini alır veya ayarlar.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Hiperlinkin araç ipucunu alır veya ayarlar.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | URL dizesini alır veya ayarlar.(Inherited from [`Hyperlink`](../hyperlink/).) |

### Ayrıca Bakınız

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


