---
title: FormatConditionType
second_title: Aspose.Cells for .NET API Referansı
description: Koşullu biçim kuralı türü.
type: docs
weight: 3580
url: /tr/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Koşullu biçim kuralı türü.

```csharp
public enum FormatConditionType
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| CellValue | `0` | Bu koşullu biçimlendirme kuralı, hücre değerini bir işleç kullanarak formülle hesaplanmış bir sonuçla karşılaştırır. |
| Expression | `1` | Bu koşullu biçimlendirme kuralı, değerlendirme için formülü içerir. Formül sonucu doğru olduğunda, hücre vurgulanır . |
| ColorScale | `2` | Bu koşullu biçimlendirme kuralı, hücrelerde derecelendirilmiş bir renk ölçeği oluşturur. |
| DataBar | `3` | Bu koşullu biçimlendirme kuralı, hücre aralığında derecelendirilmiş bir veri çubuğu görüntüler. |
| IconSet | `4` | Bu koşullu biçimlendirme kuralı, simgeleri değerlerine göre hücrelere uygular. |
| Top10 | `5` | Bu koşullu biçimlendirme kuralı, belirtilen şekilde, değerleri üst N veya alt N parantezine giren hücreleri vurgular. |
| UniqueValues | `6` | Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerlerini vurgular. |
| DuplicateValues | `7` | Bu koşullu biçimlendirme kuralı, yinelenen değerlerini vurgular. |
| ContainsText | `8` | Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevini kullanmaya eşdeğerdir. |
| NotContainsText | `9` | Bu koşullu biçimlendirme kuralı, verilen metni içermeyen hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevini kullanmaya eşdeğerdir. |
| BeginsWith | `10` | Bu koşullu biçimlendirme kuralı, verilen metinle başlayan aralığındaki hücreleri vurgular. LEFT() sayfa işlevini kullanarak ve değerleri karşılaştırarak ile eşdeğerdir. |
| EndsWith | `11` | Bu koşullu biçimlendirme kuralı, verilen metinle ile biten hücreleri vurgular. RIGHT() sayfa işlevini kullanmaya ve değerleri karşılaştırmaya eşdeğerdir. |
| ContainsBlanks | `12` | Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücrenin yalnızca TRIM()'in kaldıracağı karakterlerini içermesi durumunda boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| NotContainsBlanks | `13` | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. This , hücrenin yalnızca TRIM()'in kaldıracağı karakterleri içermesi durumunda boş olarak kabul edildiği anlamına gelir. An boş hücre de boş olarak kabul edilir. |
| ContainsErrors | `14` | Bu koşullu biçimlendirme kuralı, formül hataları olan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevini kullanmaya eşdeğerdir. |
| NotContainsErrors | `15` | Bu koşullu biçimlendirme kuralı, hücreleri formül hatası olmadan vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevini kullanmaya eşdeğerdir. |
| TimePeriod | `16` | Bu koşullu biçimlendirme kuralı, belirtilen zaman aralığındaki tarihleri içeren cell öğesini vurgular. Hücrenin temel alınan değeri değerlendirilir, bu nedenle hücresinin, değerlendirilecek tarihi olarak biçimlendirilmesi gerekmez. Örneğin, 38913 değerini içeren bir hücreyle, koşullu biçim uygulanacaksa kuralı 14.07.2006 değerini gerektiriyorsa. |
| AboveAverage | `17` | Bu koşullu biçimlendirme kuralı, aralığındaki tüm değerler için ortalamanın üstünde veya altında olan hücreleri vurgular. |

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
