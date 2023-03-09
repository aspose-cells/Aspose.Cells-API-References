---
title: FormatConditionType numaralandırma
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 2100
url: /tr/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType numaralandırma
Koşullu biçim kural türü.



FormatConditionType türü aşağıdaki üyeleri gösterir:

###  alanlar
| Alan| Tanım|
| :- | :- |
| CELL_VALUE | Bu koşullu biçimlendirme kuralı, bir hücre değerini karşılaştırır<br/> bir operatör kullanılarak formül hesaplanan sonuca.|
| EXPRESSION | Bu koşullu biçimlendirme kuralı,<br/>Formül sonucu doğru olduğunda, hücre<br/> vurgulanmıştır.|
| COLOR_SCALE | Bu koşullu biçimlendirme kuralı, dereceli bir biçimlendirme oluşturur.<br/> hücrelerde renk skalası.|
| DATA_BAR | Bu koşullu biçimlendirme kuralı, derecelendirilmiş bir<br/> hücre aralığındaki veri çubuğu.|
| ICON_SET |Bu koşullu biçimlendirme kuralı, simgeleri hücrelere uygular<br/> değerlerine göre.|
| TOP10 | Bu koşullu biçimlendirme kuralı,<br/>değerler üst N veya alt N köşeli parantez içine düşer;<br/> belirtildi.|
| UNIQUE_VALUES | Bu koşullu biçimlendirme kuralı, benzersiz özellikleri vurgular<br/> aralığındaki değerler.|
| DUPLICATE_VALUES | Bu koşullu biçimlendirme kuralı yinelenenleri vurgular<br/> değerler.|
| CONTAINS_TEXT | Bu koşullu biçimlendirme kuralı hücreleri vurgular<br/>verilen metni içerir. SEARCH() işlevinin kullanılmasına eşdeğerdir.<br/>hücrenin içerip içermediğini belirlemek için sayfa işlevi<br/> Metin.|
| NOT_CONTAINS_TEXT | Bu koşullu biçimlendirme kuralı,<br/>verilen metni içermez.<br/>hücrenin içerip içermediğini belirlemek için sayfa işlevi<br/> metin ya da değil.|
| BEGINS_WITH | Bu koşullu biçimlendirme kuralı,<br/>verilen metinle başlayan aralık.<br/> LEFT() sayfa işlevini kullanma ve değerleri karşılaştırma.|
| ENDS_WITH | Bu koşullu biçimlendirme kuralı, biten hücreleri vurgular<br/>verilen metinle. RIGHT() sayfasını kullanmaya eşdeğerdir.<br/> fonksiyon ve karşılaştırma değerleri.|
| CONTAINS_BLANKS | Bu koşullu biçimlendirme kuralı,<br/>tamamen boştur. LEN(TRIM()) kullanımına eşdeğerdir.<br/>Bunun anlamı, eğer hücre sadece karakter içeriyorsa<br/>TRIM() kaldırılırsa, boş kabul edilir.<br/> Boş bir hücre de boş kabul edilir.|
| NOT_CONTAINS_BLANKS | Bu koşullu biçimlendirme kuralı,<br/>LEN(TRIM()) kullanımına eşdeğerdir.<br/>hücrenin yalnızca şu karakterleri içermesi anlamına gelir:<br/>TRIM() kaldırır, sonra boş kabul edilir.<br/> boş hücreler de boş kabul edilir.|
| CONTAINS_ERRORS | Bu koşullu biçimlendirme kuralı, şu özelliklere sahip hücreleri vurgular:<br/>formül hataları ISERROR() sayfası kullanmaya eşdeğerdir.<br/> formül hatası olup olmadığını belirleme işlevi.|
| NOT_CONTAINS_ERRORS | Bu koşullu biçimlendirme kuralı hücreleri vurgular<br/>formül hatası olmadan. ISERROR() kullanımına eşdeğerdir.<br/> formül hatası olup olmadığını belirlemek için sayfa işlevi.|
| TIME_PERIOD | Bu koşullu biçimlendirme kuralı hücreleri vurgular<br/>belirtilen zaman dilimindeki tarihleri içeren.<br/>hücrenin temel değeri değerlendirilir, bu nedenle<br/>hücrenin tarih olarak biçimlendirilmesi gerekmez<br/>Örneğin, şunu içeren bir hücre ile<br/>38913 değeri, şu durumlarda koşullu biçim uygulanacaktır:<br/> kural 7/14/2006 değerini gerektirir.|
| ABOVE_AVERAGE | Bu koşullu biçimlendirme kuralı,<br/>içindeki tüm değerler için ortalamanın üstünde veya altında<br/> menzil.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
