---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.FormatConditionType enum. Koşullu biçim kuralı tipi"
type: docs
url: /tr/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Koşullu biçim kuralı türü.

```csharp
public enum FormatConditionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| CellValue | `0` | Bu koşullu biçimlendirme kuralı, bir hücre değerini bir formülün hesaplanan sonucu ile bir operatör kullanarak karşılaştırır. |
| Expression | `1` | Bu koşullu biçimlendirme kuralı, değerlendirilmesi gereken bir formül içerir. Formül sonucu doğru olduğunda, hücre vurgulanır. |
| ColorScale | `2` | Bu koşullu biçimlendirme kuralı, hücrelerde kademeli bir renk ölçeği oluşturur. |
| DataBar | `3` | Bu koşullu biçimlendirme kuralı, hücre aralığında kademeli bir veri çubuğu gösterir. |
| IconSet | `4` | Bu koşullu biçimlendirme kuralı, hücreleri değerlerine göre simgelerle işaretler. |
| Top10 | `5` | Bu koşullu biçimlendirme kuralı, belirtilen şekilde değerleri üst N veya alt N aralığına düşen hücreleri vurgular. |
| UniqueValues | `6` | Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerleri vurgular. |
| DuplicateValues | `7` | Bu koşullu biçimlendirme kuralı, yinelenen değerleri vurgular. |
| ContainsText | `8` | Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevinin kullanılmasına eşdeğerdir. |
| NotContainsText | `9` | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| BeginsWith | `10` | Bu koşullu biçimlendirme kuralı, verilen metinle başlayan hücreleri aralıkta vurgular. LEFT() sayfa işlevinin kullanılması ve değerlerin karşılaştırılmasıyla eşdeğerdir. |
| EndsWith | `11` | Bu koşullu biçimlendirme kuralı, verilen metinle biten hücreleri vurgular. RIGHT() sayfa işlevinin kullanılması ve değerlerin karşılaştırılmasıyla eşdeğerdir. |
| ContainsBlanks | `12` | Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| NotContainsBlanks | `13` | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| ContainsErrors | `14` | Bu koşullu biçimlendirme kuralı, formül hatası olan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevinin kullanılmasına eşdeğerdir. |
| NotContainsErrors | `15` | Bu koşullu biçimlendirme kuralı, formül hatası olmayan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevinin kullanılmasına eşdeğerdir. |
| TimePeriod | `16` | Bu koşullu biçimlendirme kuralı, belirtilen zaman dilimindeki tarihleri içeren hücreleri vurgular. Hücrenin temel değeri değerlendirilir, bu nedenle hücrenin tarih olarak biçimlendirilmiş olması değerlendirme için gerekli değildir. Örneğin, değeri 38913 olan bir hücrede, kural 7/14/2006 tarihini gerektiriyorsa koşullu biçimlendirme uygulanır. |
| AboveAverage | `17` | Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki veya altındaki hücreleri vurgular. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


