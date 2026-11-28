---
title: "Sınıf Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Style sınıfı. Yazı tipi rengi, hizalama, kenarlık vb. gibi Excel belgelerinin görüntü stilini temsil eder"
type: docs
url: /tr/net/aspose.cells.griddesktop/style/
---
## Style class

Excel belgesinin görüntü stilini temsil eder; örneğin yazı tipi, renk, hizalama, kenarlık vb.

```csharp
public class Style
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Style](style/)(GridDesktop) | Denetim için yeni bir Style oluştur |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Hücre arka plan rengini alır veya ayarlar; stil deseni katı (solid) olarak ayarlanmamışsa etkili olur |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Hücre gölgelendirme rengini alır veya ayarlar. Desen none olduğunda Color.Empty döner; desen BackgroundType.Solid olduğunda ForegroundColor döner; diğer durumlarda BackgroundColor döner. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Bu stil nesnesinin özel sayı formatı dizesini temsil eder. Özel sayı formatı ayarlanmamışsa (örneğin, sayı formatı yerleşik ise), \"\" döndürülür. |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Bir [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/) nesnesi alır. |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Bir stilin ön plan rengini alır veya ayarlar. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Yatay hizalama özelliğini alır veya ayarlar. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Hücre veya aralık için m_IndentLevel seviyesini temsil eder. Yalnızca 0 ile 15 arasında bir tam sayı olabilir. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Sayıların ve tarihlerin görüntüleme biçimini alır veya ayarlar. Biçimlendirme desenleri farklı bölgeler için farklıdır. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Hücre arka planı desen türünü alır veya ayarlar. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Metin döndürme açısını temsil eder. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Metnin kullanılabilir sütun genişliğine sığacak şekilde otomatik olarak küçültülüp küçültülmediğini temsil eder. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Metin yönü özelliğini alır veya ayarlar. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Bir hücre içindeki metnin kaydırılıp kaydırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Dikey hizalama özelliğini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Bu nesnenin bir kopyasını oluşturur ve döndürür. **NOTE:** Adlandırılmış bir stili klonlarsanız, ad klonlanmaz çünkü stil adı benzersiz olmalıdır. Bu nedenle, klonlanan stil orijinal stil ile "equals to" olmayacaktır. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Belirtilen kenarlığın rengini ayarlar. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Belirtilen kenarlığın çizgi tipini ayarlar. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


