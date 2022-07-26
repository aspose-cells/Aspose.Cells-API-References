---
title: Style
second_title: Aspose.Cells for .NET API Referansı
description: Yazı tipi renk hizalama kenarlık vb. gibi excel belgesinin görüntüleme stilini temsil eder. Stil nesnesi özellikler olarak tüm stil özniteliklerini yazı tipi sayı biçimi hizalama vb. içerir.
type: docs
weight: 5750
url: /tr/net/aspose.cells/style/
---
## Style class

Yazı tipi, renk, hizalama, kenarlık vb. gibi excel belgesinin görüntüleme stilini temsil eder. Stil nesnesi, özellikler olarak tüm stil özniteliklerini (yazı tipi, sayı biçimi, hizalama vb.) içerir.

```csharp
public class Style
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | 32 bit ARGB değeriyle arka plan rengini alır ve ayarlar. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Bir stilin arka plan rengini alır veya ayarlar. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Arka plan tema rengini alır ve ayarlar. |
| [Borders](../../aspose.cells/style/borders) { get; } | [`BorderCollection`](../bordercollection) tarzın. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Sayı biçimi için kültüre bağlı kalıp dizesini alır ve ayarlar. Bu nesne için herhangi bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşikse, yerleşik sayıya karşılık gelen kalıp dizesi döndürülür. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Bu stil nesnesinin özel sayı biçimi dizesini temsil eder. Özel sayı biçimi ayarlanmazsa (Örneğin, sayı biçimi yerleşiktir), "" döndürülür. |
| [Font](../../aspose.cells/style/font) { get; } | [`Font`](./font) nesne. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | 32 bit ARGB değeriyle ön plan rengini alır ve ayarlar. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Bir stilin ön plan rengini alır veya ayarlar. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Ön plan tema rengini alır ve ayarlar. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Stil için ayarlanmış kenarlıklar olup olmadığını kontrol eder. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Hücre veya aralığın girinti düzeyini temsil eder. Yalnızca 0 ile 250. arasında bir tam sayı olabilir |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Sayı biçimi için kültürden bağımsız kalıp dizesini alır. Bu nesne için herhangi bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşikse, yerleşik sayıya karşılık gelen kalıp dizesi döndürülür. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Sayı biçiminin bir tarih biçimi olup olmadığını gösterir. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Hücre gölgelendirmesinin bir degrade deseni olup olmadığını gösterir. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Metnin son satırında hücrelerin hizalanmış veya dağıtılmış hizalamanın kullanılması gerekip gerekmediğini gösterir. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Bir hücrenin değiştirilip değiştirilemeyeceğini gösteren bir değer alır veya ayarlar. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Sayı biçiminin yüzde biçimi olup olmadığını gösterir. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Bir hücre içindeki metnin sarılıp sarılmadığını gösteren bir değer alır veya ayarlar. |
| [Name](../../aspose.cells/style/name) { get; set; } | Stilin adını alır veya ayarlar. |
| [Number](../../aspose.cells/style/number) { get; set; } | Sayıların ve tarihlerin görüntülenme biçimini alır veya ayarlar. Biçimlendirme kalıpları, farklı bölgeler için farklıdır. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Bu stilin üst stilini alır. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Hücre arka plan deseni türünü alır veya ayarlar. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Metin döndürme açısını temsil eder. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Metnin, mevcut sütun genişliğine sığacak şekilde otomatik olarak küçülüp küçülmediğini temsil eder. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Metin okuma sırasını temsil eder. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Bir hücredeki metnin dikey hizalama türünü alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Verileri başka bir nesne stilinden kopyalar |
| override [Equals](../../aspose.cells/style/equals)(object) | İki Stil örneğinin eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Bir Style nesnesi için karma işlevi olarak hizmet eder. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | İki renkli gradyan ayarını alın. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. ConditionalFormattings stili için, bu stilin belirtilen özelliklerinin bir hücreye ConditionalFormattings uygulanırken kullanılması gerekip gerekmediğini kontrol etmek için kullanılır. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Stilin sınırlarını ayarlar. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Bir hücrenin Özel sayı biçimi dizesini ayarlar. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Arka plan rengini ayarlar. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar. |
| [Update](../../aspose.cells/style/update)() | Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygulayın. Stili değiştirmeyi bitirdikten sonra "tamam" düğmesini tıklamak gibi çalışır. Yalnızca adlandırılmış stil için geçerlidir. |

### Örnekler

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
