---
title: "Style Sınıfı"
linktitle: "Style"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Style sınıfı. Go'da style'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/style/
---

## Style class

Excel belgesinin görüntü stilini temsil eder, örneğin yazı tipi, renk, hizalama, kenarlık vb.The Style nesnesi, tüm stil özelliklerini (yazı tipi, sayı biçimi, hizalama vb.) özellikler olarak içerir.

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Arka plan tema rengini alır ve ayarlar. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Arka plan tema rengini alır ve ayarlar. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Ön plan tema rengini alır ve ayarlar. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Ön plan tema rengini alır ve ayarlar. |
| [GetName](./getname/) | Stil adını alır veya ayarlar. |
| [SetName](./setname/) | Stil adını alır veya ayarlar. |
| [GetPattern](./getpattern/) | Hücre arka plan desen türünü alır veya ayarlar. |
| [SetPattern](./setpattern/) | Hücre arka plan desen türünü alır veya ayarlar. |
| [SetPatternColor](./setpatterncolor/) | Arka plan rengini ayarlar. |
| [GetBorders](./getborders/) | Stilin BorderCollection'ını alır. |
| [GetBackgroundColor](./getbackgroundcolor/) | Bir stilin arka plan rengini alır veya ayarlar. |
| [SetBackgroundColor](./setbackgroundcolor/) | Bir stilin arka plan rengini alır veya ayarlar. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | 32-bit ARGB değeriyle arka plan rengini alır ve ayarlar. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | 32-bit ARGB değeriyle arka plan rengini alır ve ayarlar. |
| [GetForegroundColor](./getforegroundcolor/) | Bir stilin ön plan rengini alır veya ayarlar. |
| [SetForegroundColor](./setforegroundcolor/) | Bir stilin ön plan rengini alır veya ayarlar. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | 32-bit ARGB değeriyle ön plan rengini alır ve ayarlar. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | 32-bit ARGB değeriyle ön plan rengini alır ve ayarlar. |
| [Copy](./copy/) | Başka bir stil nesnesinden verileri kopyalar |
| [GetHasBorders](./gethasborders/) | Stil için kenarlıkların ayarlanıp ayarlanmadığını kontrol eder. |
| [GetParentStyle](./getparentstyle/) | Bu stilin üst stilini alır. |
| [Update](./update/) | Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygula. Stil üzerinde değişiklikleri tamamladıktan sonra "tamam" düğmesine tıklamak gibi çalışır. Yalnızca adlandırılmış stil için geçerlidir. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsFontApplied](./isfontapplied/) | Yazı tipi biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsFontApplied](./setisfontapplied/) | Yazı tipi biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsAlignmentApplied](./isalignmentapplied/) | Hizalama biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Hizalama biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsBorderApplied](./isborderapplied/) | Kenarlık biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsBorderApplied](./setisborderapplied/) | Kenarlık biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsFillApplied](./isfillapplied/) | Dolgu biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsFillApplied](./setisfillapplied/) | Dolgu biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsProtectionApplied](./isprotectionapplied/) | Koruma biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Koruma biçimlendirmenin uygulanıp uygulanmayacağını belirt. |
| [IsModified](./ismodified/) | Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. Hücreye ConditionalFormattings uygulanırken bu stilin belirtilen özelliklerinin kullanılıp kullanılmayacağını kontrol etmek için ConditionalFormattings stilinde kullanılır. |
| [Equals](./equals/) | İki Style örneğinin eşit olup olmadığını belirler. |
| [GetHashCode](./gethashcode/) | Bir Style nesnesi için hash işlevi olarak hizmet verir. |
| [GetIndentLevel](./getindentlevel/) | Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir. |
| [SetIndentLevel](./setindentlevel/) | Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir. |
| [GetFont](./getfont/) | Bir Font nesnesi alır. |
| [GetRotationAngle](./getrotationangle/) | Metin döndürme açısını temsil eder. |
| [SetRotationAngle](./setrotationangle/) | Metin döndürme açısını temsil eder. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar. |
| [GetVerticalAlignment](./getverticalalignment/) | Bir hücredeki metnin dikey hizalama türünü alır veya ayarlar. |
| [SetVerticalAlignment](./setverticalalignment/) | Bir hücredeki metnin dikey hizalama türünü alır veya ayarlar. |
| [IsTextWrapped](./istextwrapped/) | Bir hücredeki metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [SetIsTextWrapped](./setistextwrapped/) | Bir hücredeki metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [GetNumber](./getnumber/) | Sayıların ve tarihlerin görüntüleme biçimini alır veya ayarlar. Biçimlendirme kalıpları farklı bölgeler için farklıdır. |
| [SetNumber](./setnumber/) | Sayıların ve tarihlerin görüntüleme biçimini alır veya ayarlar. Biçimlendirme kalıpları farklı bölgeler için farklıdır. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Stilin kenarlıklarını ayarlar. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Stilin kenarlıklarını ayarlar. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Ana hat kenarlıklarını ayarla |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Ana hat kenarlıklarını ayarla |
| [IsLocked](./islocked/) | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [SetIsLocked](./setislocked/) | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Bir hücrenin Özel sayı biçim dizesini ayarlar. |
| [GetCustom](./getcustom/) | Bu stil nesnesinin özel sayı biçim dizesini temsil eder. Özel sayı biçimi ayarlanmamışsa (örneğin, sayı biçimi yerleşik ise), \"\" döndürülür. |
| [SetCustom_String](./setcustom_string/) | Bu stil nesnesinin özel sayı biçim dizesini temsil eder. Özel sayı biçimi ayarlanmamışsa (örneğin, sayı biçimi yerleşik ise), \"\" döndürülür. |
| [GetCultureCustom](./getculturecustom/) | Sayı biçimi için kültüre bağlı kalıp dizesini alır ve ayarlar. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen kalıp dizesi döndürülür. |
| [SetCultureCustom](./setculturecustom/) | Sayı biçimi için kültüre bağlı kalıp dizesini alır ve ayarlar. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen kalıp dizesi döndürülür. |
| [GetInvariantCustom](./getinvariantcustom/) | Sayı biçimi için kültür bağımsız kalıp dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen kalıp dizesi döndürülür. |
| [IsFormulaHidden](./isformulahidden/) | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [SetIsFormulaHidden](./setisformulahidden/) | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [GetShrinkToFit](./getshrinktofit/) | Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçültülüp küçültülmeyeceğini temsil eder. |
| [SetShrinkToFit](./setshrinktofit/) | Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçültülüp küçültülmeyeceğini temsil eder. |
| [GetTextDirection](./gettextdirection/) | Metin okuma sırasını temsil eder. |
| [SetTextDirection](./settextdirection/) | Metin okuma sırasını temsil eder. |
| [IsJustifyDistributed](./isjustifydistributed/) | Metnin son satırında hücrelerin iki yana yaslanmış veya dağıtılmış hizalamasının kullanılıp kullanılmayacağını gösterir. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Metnin son satırında hücrelerin iki yana yaslanmış veya dağıtılmış hizalamasının kullanılıp kullanılmayacağını gösterir. |
| [GetQuotePrefix](./getquoteprefix/) | Hücre değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [SetQuotePrefix](./setquoteprefix/) | Hücre değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [IsGradient](./isgradient/) | Hücre gölgelendirmenin bir degrade kalıbı olup olmadığını gösterir. |
| [SetIsGradient](./setisgradient/) | Hücre gölgelendirmenin bir degrade kalıbı olup olmadığını gösterir. |
| [SetTwoColorGradient](./settwocolorgradient/) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | İki renkli degrade ayarını al. |
| [IsPercent](./ispercent/) | Sayı biçiminin yüzde biçimi olup olmadığını gösterir. |
| [IsDateTime](./isdatetime/) | Sayı biçiminin tarih biçimi olup olmadığını gösterir. |
| [IsCheckBox](./ischeckbox/) | Bir onay kutusu stili olup olmadığını gösterir |
| [SetIsCheckBox](./setischeckbox/) | Bir onay kutusu stili olup olmadığını gösterir |
| [ToJson](./tojson/) | Stili JSON yapı verisine dönüştür. |
| [GetLeftBorder](./getleftborder/) | Sol kenarlığı al. |
| [GetRightBorder](./getrightborder/) | Sağ kenarlığı al. |
| [GetTopBorder](./gettopborder/) | Üst kenarı alır. |
| [GetBottomBorder](./getbottomborder/) | Alt kenarı alır. |
