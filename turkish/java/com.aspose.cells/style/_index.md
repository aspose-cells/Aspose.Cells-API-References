---
title: "Style"
second_title: "Aspose.Cells for Java API Referansı"
description: "Excel belgelerinin görüntü stilini, örneğin yazı tipi, renk, hizalama, kenarlık vb. temsil eder."
type: docs
url: /tr/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Excel belgesinin görüntü stilini, örneğin yazı tipi, renk, hizalama, kenarlık vb. temsil eder. Style nesnesi, tüm stil özelliklerini (yazı tipi, sayı biçimi, hizalama vb.) özellikler olarak içerir.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Style()](#Style--) | Yeni bir [Style](../../com.aspose.cells/style) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Başka bir stil nesnesinden verileri kopyalar |
| [equals(Object obj)](#equals-java.lang.Object-) | İki Style örneğinin eşit olup olmadığını belirler. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | 32-bit ARGB değeriyle arka plan rengini alır. |
| [getBackgroundColor()](#getBackgroundColor--) | Bir stilin arka plan rengini alır. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Arka plan tema rengini alır. |
| [getBorders()](#getBorders--) | Stilin [BorderCollection](../../com.aspose.cells/bordercollection) nesnesini alır. |
| [getBottomBorder()](#getBottomBorder--) | Alt kenarı alır. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Sayı biçimi için kültüre bağlı desen dizesini alır. |
| [getCustom()](#getCustom--) | Bu stil nesnesinin özel sayı biçimi dizesini temsil eder. |
| [getFont()](#getFont--) | Bir [getFont()](../../com.aspose.cells/style\#getFont--) nesnesi alır. |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | 32-bit ARGB değeriyle ön plan rengini alır. |
| [getForegroundColor()](#getForegroundColor--) | Bir stilin ön plan rengini alır. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Ön plan tema rengini alır. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Bir hücredeki metnin yatay hizalama türünü alır. |
| [getIndentLevel()](#getIndentLevel--) | Hücre veya aralık için girinti seviyesini temsil eder. |
| [getInvariantCustom()](#getInvariantCustom--) | Sayı biçimi için kültür bağımsız desen dizesini alır. |
| [getLeftBorder()](#getLeftBorder--) | Sol kenarı alır. |
| [getName()](#getName--) | Stil adını alır. |
| [getNumber()](#getNumber--) | Sayıların ve tarihlerin görüntüleme biçimini alır. |
| [getParentStyle()](#getParentStyle--) | Bu stilin üst stilini alır. |
| [getPattern()](#getPattern--) | Hücre arka planı desen türünü alır. |
| [getQuotePrefix()](#getQuotePrefix--) | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [getRightBorder()](#getRightBorder--) | Sağ kenarı alır. |
| [getRotationAngle()](#getRotationAngle--) | Metin döndürme açısını temsil eder. |
| [getShrinkToFit()](#getShrinkToFit--) | Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçülüp küçülmediğini temsil eder. |
| [getTextDirection()](#getTextDirection--) | Metin okuma sırasını temsil eder. |
| [getTopBorder()](#getTopBorder--) | Üst kenarı alır. |
| [getTwoColorGradient()](#getTwoColorGradient--) | İki renkli degrade ayarını al. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | İki renkli degrade ayarını al. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Bir hücredeki metnin dikey hizalama türünü alır. |
| [hasBorders()](#hasBorders--) | Stil için kenarların ayarlanıp ayarlanmadığını denetler. |
| [hashCode()](#hashCode--) | Bir Style nesnesi için hash işlevi olarak hizmet eder. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [isBorderApplied()](#isBorderApplied--) | Kenar biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [isCheckBox()](#isCheckBox--) | Bir onay kutusu stili olup olmadığını gösterir. |
| [isDateTime()](#isDateTime--) | Sayı biçiminin tarih biçimi olup olmadığını gösterir. |
| [isFillApplied()](#isFillApplied--) | Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [isFontApplied()](#isFontApplied--) | Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [isFormulaHidden()](#isFormulaHidden--) | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [isGradient()](#isGradient--) | Hücre gölgelendirmenin bir degrade desen olup olmadığını gösterir. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Hücrelerin son satırdaki metin için iki yana yaslı veya dağıtılmış hizalamanın kullanılıp kullanılmayacağını gösterir. |
| [isLocked()](#isLocked--) | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değer alır. |
| [isModified(int modifyFlag)](#isModified-int-) | Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirtir. |
| [isPercent()](#isPercent--) | Sayısal biçimin yüzde formatı olup olmadığını gösterir. |
| [isProtectionApplied()](#isProtectionApplied--) | Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir. |
| [isTextWrapped()](#isTextWrapped--) | Bir hücre içindeki metnin kaydırılıp kaydırılmadığını gösteren bir değer alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | 32 bit ARGB değeriyle arka plan rengini ayarlar. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Bir stilin arka plan rengini ayarlar. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Arka plan tema rengini ayarlar. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Stilin kenarlıklarını ayarlar. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Stilin kenarlıklarını ayarlar. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Kenar biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Bir onay kutusu stili olup olmadığını gösterir. |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Sayısal biçim için kültüre bağlı desen dizesini ayarlar. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Bu stil nesnesinin özel sayı biçimi dizesini temsil eder. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Bir hücrenin Özel sayı biçim dizesini ayarlar. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını göster. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | 32 bit ARGB değeriyle ön plan rengini ayarlar. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Bir stilin ön plan rengini ayarlar. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Ön plan tema rengini ayarlar. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [setGradient(boolean value)](#setGradient-boolean-) | Hücre gölgelendirmenin bir degrade desen olup olmadığını gösterir. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Bir hücredeki metnin yatay hizalama türünü ayarlar. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Hücre veya aralık için girinti seviyesini temsil eder. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Hücrelerin son satırdaki metin için iki yana yaslı veya dağıtılmış hizalamanın kullanılıp kullanılmayacağını gösterir. |
| [setLocked(boolean value)](#setLocked-boolean-) | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değer ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Stilin adını ayarlar. |
| [setNumber(int value)](#setNumber-int-) | Sayıların ve tarihlerin görüntüleme biçimini ayarlar. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirtir. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Ana hat kenarlıklarını ayarla |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Ana hat kenarlıklarını ayarla |
| [setPattern(int value)](#setPattern-int-) | Hücre arka plan desen tipini ayarlar. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Arka plan rengini ayarlar. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Metin döndürme açısını temsil eder. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçülüp küçülmediğini temsil eder. |
| [setTextDirection(int value)](#setTextDirection-int-) | Metin okuma sırasını temsil eder. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Bir hücre içindeki metnin kaydırılıp kaydırılmadığını gösteren bir değer ayarlar. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Bir hücredeki metnin dikey hizalama türünü ayarlar. |
| [toJson()](#toJson--) | [Style](../../com.aspose.cells/style) öğesini JSON yapı verisine dönüştür. |
| [toString()](#toString--) |  |
| [update()](#update--) | Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygula. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Yeni bir [Style](../../com.aspose.cells/style) sınıfı örneği başlatır.

**Remarks**

NOT: Bu yapıcı artık kullanımdan kaldırılmıştır. Bunun yerine lütfen CellsFactory.CreateStyle() yöntemini kullanın. Bu özellik, Ekim 2016'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Başka bir stil nesnesinden verileri kopyalar

**Remarks**

Bu yöntem stilin adını kopyalamaz. Adı kopyalamak istiyorsanız, stil kopyalandıktan sonra lütfen aşağıdaki kodları çağırın: destStyle.Name = style.Name.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Kaynak Stil nesnesi |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


İki Style örneğinin eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Mevcut Stil nesnesiyle karşılaştırılacak Stil nesnesi. |

**Returns:**
boolean - belirtilen Nesne mevcut Nesneye eşitse true; aksi takdirde false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


32-bit ARGB değeriyle arka plan rengini alır.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Bir stilin arka plan rengini alır.

**Remarks**

Bir hücrenin rengini ayarlamak istiyorsanız, lütfen Style.ForegroundColor özelliğini kullanın. Bu özellik yalnızca hücre stil deseni none (yok) veya solid (düz) dışında olduğunda etkili olur.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Arka plan tema rengini alır.

**Remarks**

Arka plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Stilin [BorderCollection](../../com.aspose.cells/bordercollection) nesnesini alır.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Alt kenarı alır.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


Sayı biçimi için kültüre bağlı desen dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür.

**Remarks**

Yerleşik sayı biçimi için, desen içeriği (örneğin, bazı yerel ayarlar için bir yerleşik tarih biçimi "m/d/y" iken, diğer bazı yerel ayarlarda "d/m/y" olur) ve biçim belirteci (örneğin, bazı yerel ayarlar tarih biçimlendirmesinde yılı temsil etmek için 'y' haricinde bir karakter kullanır) kültüre bağlıdır; Kullanıcı tarafından belirtilen özel biçim için ise yalnızca biçim belirteçleri kültüre göre değiştirilir, biçim deseninin diğer bölümleri değiştirilmez.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Bu stil nesnesinin özel sayı biçim dizesini temsil eder. Özel sayı biçimi ayarlanmamışsa (Örneğin, sayı biçimi yerleşik ise), "" döndürülür.

**Remarks**

Döndürülen özel dize kültür bağımsızdır.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Bir [getFont()](../../com.aspose.cells/style\#getFont--) nesnesi alır.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


32-bit ARGB değeriyle ön plan rengini alır.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Bir stilin ön plan rengini alır.

**Remarks**

Color.Empty döndürülürse renk ayarı olmadığı anlamına gelir.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Ön plan tema rengini alır.

**Remarks**

Ön plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Bir hücredeki metnin yatay hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir.

**Remarks**

Metnin yatay hizalama türü sol veya sağ dışında bir değere ayarlanırsa, girinti seviyesi sıfıra sıfırlanır.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Sayı biçimi için kültür bağımsız desen dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür.

**Remarks**

Yerleşik sayı biçimleri için, döndürülen desen içeriği hâlâ kültüre bağlıdır; örneğin, bazı yerel ayarlarda "m/d/y" ve diğer bazı yerel ayarlarda "d/m/y" döner. [getCultureCustom()](../../com.aspose.cells/style\\#getCultureCustom--) ile farkı (bu aynı zamanda kültür bağımsızının ne anlama geldiğidir): biçim belirteçleri ve ayırıcılar standart olarak korunur; örneğin '/' her zaman tarih‑saat ayırıcı olarak kullanılır ve "y" her zaman "yıl" kısmı olarak kullanılır, belirli yerel ayar için başka özel bir karakter kullanılsa bile.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Sol kenarı alır.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Stil adını alır.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Sayıların ve tarihlerin görüntüleme biçimini alır. Biçimlendirme desenleri farklı bölgeler için farklıdır.

**Remarks**

Örneğin, en\\_US bölgesi için sayılarla temsil edilen biçimlendirme desenleri:

| Değer | Tür | Biçim Dizesi |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Kırmızı](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Kırmızı](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ÖÖ/ÖS` |
| 19 | Time | `h:mm:ss ÖÖ/ÖS` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Kırmızı](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Kırmızı](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Bu stilin üst stilini alır.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Hücre arka planı desen türünü alır.

Bakınız [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Sağ kenarı alır.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Metin döndürme açısını temsil eder.

**Remarks**

0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.

255 veya -90 ile 90 arasında bir değer ayarlayabilirsiniz.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçülüp küçülmediğini temsil eder.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Üst kenarı alır.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


İki renkli degrade ayarını al.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Style.GetTwoColorGradientSetting() yöntemini kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.Object[] - İki renkli degrade hakkında tüm ayarları döndürür [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


İki renkli degrade ayarını al.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Bir hücredeki metnin dikey hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Stil için kenarların ayarlanıp ayarlanmadığını denetler.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bir Style nesnesi için hash işlevi olarak hizmet eder.

**Remarks**

Bu yöntem yalnızca dahili kullanım içindir.

**Returns:**
int - Mevcut Nesne için bir karma kodu.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Kenar biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Bir onay kutusu stili olup olmadığını gösterir.

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Sayı biçiminin tarih biçimi olup olmadığını gösterir.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Hücre gölgelendirmenin bir degrade desen olup olmadığını gösterir.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Hücrelerin son satırdaki metin için iki yana yaslı veya dağıtılmış hizalamanın kullanılıp kullanılmayacağını gösterir.

**Remarks**

Bu, Doğu Asya hizalamaları için tipiktir ancak diğer bağlamlarda tipik değildir. Yalnızca dağıtılmış yatay hizalama olduğunda çalışır.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değer alır.

**Remarks**

Hücreleri kilitlemek, çalışma sayfası korunmadıkça etkisizdir.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. ConditionalFormattings stilinde, bu stilin belirtilen özelliklerinin bir hücreye ConditionalFormattings uygulanırken kullanılıp kullanılmayacağını kontrol etmek için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Stil değiştirme bayrakları |

**Returns:**
boolean - belirtilen özellikler değiştirilmişse true
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirtir.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Sayısal biçimin yüzde formatı olup olmadığını gösterir.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir.

**Remarks**

Yalnızca adlandırılmış stil için.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Bir hücre içindeki metnin kaydırılıp kaydırılmadığını gösteren bir değer alır.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


32 bit ARGB değeriyle arka plan rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Bir stilin arka plan rengini ayarlar.

**Remarks**

Bir hücrenin rengini ayarlamak istiyorsanız, lütfen Style.ForegroundColor özelliğini kullanın. Bu özellik yalnızca hücre stil deseni none (yok) veya solid (düz) dışında olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Arka plan tema rengini ayarlar.

**Remarks**

Arka plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Stilin kenarlıklarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Ayarlanacak kenarlık(lar), [BorderType](../../com.aspose.cells/bordertype) kombinasyonu olabilir. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlığın stili. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Kenarlığın rengi. |

**Returns:**
boolean - Mevcut kenarlık ayarlarının değişip değişmediği.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Stilin kenarlıklarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Ayarlanacak kenarlık(lar), [BorderType](../../com.aspose.cells/bordertype) kombinasyonu olabilir. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlığın stili. |
| borderColor | [Color](../../com.aspose.cells/color) | Kenarlığın rengi. |

**Returns:**
boolean - Mevcut kenarlık ayarlarının değişip değişmediği.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Kenar biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Bir onay kutusu stili olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Sayı biçimi için kültüre bağımlı desen dizesini ayarlar. Bu nesne için bir sayı biçimi ayarlanmamışsa, null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür.

**Remarks**

Yerleşik sayı biçimi için, desen içeriği (örneğin, bazı yerel ayarlar için bir yerleşik tarih biçimi "m/d/y" iken, diğer bazı yerel ayarlarda "d/m/y" olur) ve biçim belirteci (örneğin, bazı yerel ayarlar tarih biçimlendirmesinde yılı temsil etmek için 'y' haricinde bir karakter kullanır) kültüre bağlıdır; Kullanıcı tarafından belirtilen özel biçim için ise yalnızca biçim belirteçleri kültüre göre değiştirilir, biçim deseninin diğer bölümleri değiştirilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Bu stil nesnesinin özel sayı biçim dizesini temsil eder. Özel sayı biçimi ayarlanmamışsa (Örneğin, sayı biçimi yerleşik ise), "" döndürülür.

**Remarks**

Döndürülen özel dize kültür bağımsızdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Bir hücrenin Özel sayı biçim dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| özel | java.lang.String | Özel sayı biçim dizesi, InvariantCulture deseni olmalıdır. |
| builtinPreference | boolean | Verilen Özel sayı biçim dizesi, mevcut bölgesel ayarlarla eşleşen yerleşik sayı biçimlerinden birine uyuyorsa, sayı biçimini Özel yerine yerleşik olarak ayarlayıp ayarlamayacağını belirtir. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını göster.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


32 bit ARGB değeriyle ön plan rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Bir stilin ön plan rengini ayarlar.

**Remarks**

Color.Empty döndürülürse renk ayarı olmadığı anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Ön plan tema rengini ayarlar.

**Remarks**

Ön plan rengi bir tema rengi değilse, NULL döndürülecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Hücre gölgelendirmenin bir degrade desen olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Bir hücredeki metnin yatay hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir.

**Remarks**

Metnin yatay hizalama türü sol veya sağ dışında bir değere ayarlanırsa, girinti seviyesi sıfıra sıfırlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Hücrelerin son satırdaki metin için iki yana yaslı veya dağıtılmış hizalamanın kullanılıp kullanılmayacağını gösterir.

**Remarks**

Bu, Doğu Asya hizalamaları için tipiktir ancak diğer bağlamlarda tipik değildir. Yalnızca dağıtılmış yatay hizalama olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değer ayarlar.

**Remarks**

Hücreleri kilitlemek, çalışma sayfası korunmadıkça etkisizdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Stilin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Sayıların ve tarihlerin görüntüleme biçimini ayarlar. Biçimlendirme desenleri farklı bölgeler için farklıdır.

**Remarks**

Örneğin, en\\_US bölgesi için sayılarla temsil edilen biçimlendirme desenleri:

| Değer | Tür | Biçim Dizesi |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Kırmızı](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Kırmızı](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ÖÖ/ÖS` |
| 19 | Time | `h:mm:ss ÖÖ/ÖS` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Kırmızı](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Kırmızı](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Sayısal biçimlendirmenin uygulanıp uygulanmayacağını belirtir.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Ana hat kenarlıklarını ayarla

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlıkların türü. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Kenarlıkların rengi |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Ana hat kenarlıklarını ayarla

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlıkların türü. |
| borderColor | [Color](../../com.aspose.cells/color) | Kenarlıkların rengi |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Hücre arka plan desen tipini ayarlar.

Bakınız [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Arka plan rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Desen. |
| color1 | [Color](../../com.aspose.cells/color) | Ön plan rengi. |
| color2 | [Color](../../com.aspose.cells/color) | Arka plan rengi. Yalnızca desen BackgroundType.None ve BackgroundType.Solid olmadığında çalışır. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirtir.

**Remarks**

Yalnızca adlandırılmış stil için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Metin döndürme açısını temsil eder.

**Remarks**

0: Döndürülmemiş.

255: Yukarıdan Aşağıya.

\-90: Aşağı.

90: Yukarı.

255 veya -90 ile 90 arasında bir değer ayarlayabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Metnin mevcut sütun genişliğine sığacak şekilde otomatik olarak küçülüp küçülmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Metin okuma sırasını temsil eder.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Bir hücre içindeki metnin kaydırılıp kaydırılmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Bir hücredeki metnin dikey hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


[Style](../../com.aspose.cells/style) öğesini JSON yapı verisine dönüştür.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygula. Stil üzerinde değişiklik yaptıktan sonra "tamam" düğmesine tıklamaya benzer şekilde çalışır. Yalnızca adlandırılmış stil için geçerlidir.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

