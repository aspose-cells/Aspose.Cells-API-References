---
title: "FormatConditionType Enum"
linktitle: "FormatConditionType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FormatConditionType enum. Go dilinde formatconditiontype'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

Koşullu biçim kuralı türü.

```go

type FormatConditionType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [CellValue](./cellvalue/) | Bu koşullu biçimlendirme kuralı, bir hücre değerini bir formülün hesaplanan sonucu ile bir operatör kullanarak karşılaştırır. |
| [Expression](./expression/) | Bu koşullu biçimlendirme kuralı değerlendirilmek üzere bir formül içerir. Formül sonucu doğru olduğunda hücre vurgulanır. |
| [Top10](./top10/) | Bu koşullu biçimlendirme kuralı, değerleri belirtilen üst N veya alt N aralığına düşen hücreleri vurgular. |
| [UniqueValues](./uniquevalues/) | Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerleri vurgular. |
| [DuplicateValues](./duplicatevalues/) | Bu koşullu biçimlendirme kuralı, yinelenen değerleri vurgular. |
| [ContainsText](./containstext/) | Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa fonksiyonunu kullanmaya eşdeğerdir. |
| [NotContainsText](./notcontainstext/) | Bu koşullu biçimlendirme kuralı, verilen metni içermeyen hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa fonksiyonunu kullanmaya eşdeğerdir. |
| [BeginsWith](./beginswith/) | Bu koşullu biçimlendirme kuralı, verilen metinle başlayan hücreleri aralıkta vurgular. LEFT() sayfa fonksiyonunu kullanarak değerleri karşılaştırmaya eşdeğerdir. |
| [EndsWith](./endswith/) | Bu koşullu biçimlendirme kuralı, verilen metinle biten hücreleri vurgular. RIGHT() sayfa fonksiyonunu kullanarak değerleri karşılaştırmaya eşdeğerdir. |
| [ContainsBlanks](./containsblanks/) | Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in sileceği karakterleri içeriyorsa boş sayılacağı anlamına gelir. Boş bir hücre de boş kabul edilir. |
| [NotContainsBlanks](./notcontainsblanks/) | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in sileceği karakterleri içeriyorsa boş sayılacağı anlamına gelir. Boş bir hücre de boş kabul edilir. |
| [ContainsErrors](./containserrors/) | Bu koşullu biçimlendirme kuralı, formül hatası olan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa fonksiyonunu kullanmaya eşdeğerdir. |
| [NotContainsErrors](./notcontainserrors/) | Bu koşullu biçimlendirme kuralı, formül hatası olmayan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa fonksiyonunu kullanmaya eşdeğerdir. |
| [TimePeriod](./timeperiod/) | Bu koşullu biçimlendirme kuralı, belirtilen zaman dilimindeki tarihleri içeren hücreleri vurgular. Hücrenin temel değeri değerlendirilir, bu yüzden hücrenin tarih olarak biçimlendirilmiş olması değerlendirme için gerekli değildir. Örneğin, değeri 38913 olan bir hücrede kural 14/07/2006 tarihini gerektiriyorsa koşullu biçimlendirme uygulanır. |
| [AboveAverage](./aboveaverage/) | Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerinde veya altında olan hücreleri vurgular. |
| [ColorScale](./colorscale/) | Bu koşullu biçimlendirme kuralı, hücrelerde bir gradatedcolor ölçeği oluşturur. |
| [DataBar](./databar/) | Bu koşullu biçimlendirme kuralı, hücre aralığında bir gradateddata çubuğu gösterir. |
| [IconSet](./iconset/) | Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular. |
