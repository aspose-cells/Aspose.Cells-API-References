---
title: "GridPicture"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir elektronik tabloda tek bir resmi temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Bir elektronik tabloda tek bir resmi temsil eden nesneyi kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Şekle bir hiperlink ekler. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Resmi sağ üst köşeye taşır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Bir [GridShape](../../com.aspose.gridweb/gridshape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [getBorderLineColor()](#getBorderLineColor--) | Bir resmin kenar çizgisinin [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [getBorderWeight()](#getBorderWeight--) | Bir resmin kenar çizgisinin kalınlığını pt biriminde alır. |
| [getBottom()](#getBottom--) | Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Resmin verisini alır. |
| [getHeight()](#getHeight--) | Şeklin yüksekliğini piksel biriminde temsil eder. |
| [getHeightCM()](#getHeightCM--) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [getHeightInch()](#getHeightInch--) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [getHeightPt()](#getHeightPt--) | Şeklin yüksekliğini puan biriminde temsil eder. |
| [getHeightScale()](#getHeightScale--) | Orijinal resim yüksekliğinin yüzde biriminde yükseklik ölçeğini alır. |
| [getHtmlText()](#getHtmlText--) | Bu metin kutusunda veri ve bazı biçimlendirmeleri içeren html dizesini alır. |
| [getHyperlink()](#getHyperlink--) | Şeklin köprü bağlantısını alır. |
| [getID()](#getID--) | Resmin kimliğini alır / ayarlar. |
| [getImageFormat()](#getImageFormat--) | Resmin görüntü formatını alır. |
| [getLeft()](#getLeft--) | Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder. |
| [getLeftCM()](#getLeftCM--) | Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder. |
| [getLeftInch()](#getLeftInch--) | Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder. |
| [getLeftToCorner()](#getLeftToCorner--) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder. |
| [getLinkedCell()](#getLinkedCell--) | Denetimin değerine bağlı çalışma sayfası aralığını alır. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Şeklin sağ alt köşe sütunundan yatay kaymasını alır. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Şeklin sağ alt köşe satırından dikey kaymasını alır. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Sağ alt köşe sütun indeksini temsil eder. |
| [getLowerRightRow()](#getLowerRightRow--) | Sağ alt köşe satır indeksini temsil eder. |
| [getName()](#getName--) | Şeklin adını alır. |
| [getOriginalHeight()](#getOriginalHeight--) | Resmin orijinal yüksekliğini alır. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Resmin orijinal yüksekliğini santimetre biriminde alır. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Resmin orijinal yüksekliğini, inç biriminde alır. |
| [getOriginalWidth()](#getOriginalWidth--) | Resmin orijinal genişliğini alır. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Resmin orijinal genişliğini, santimetre biriminde alır. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Resmin orijinal genişliğini, inç biriminde alır. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir. |
| [getRight()](#getRight--) | Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder. |
| [getRotationAngle()](#getRotationAngle--) | Şeklin dönüşünü alır. |
| [getSourceFullName()](#getSourceFullName--) | Bağlantılı görüntünün kaynak dosyasının yolunu ve adını alır. |
| [getText()](#getText--) | Bu TextBox nesnesindeki dizeyi temsil eder. |
| [getTitle()](#getTitle--) | Mevcut şekil nesnesinin başlığını (altyazısını) belirtir. |
| [getTop()](#getTop--) | Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| [getTopCM()](#getTopCM--) | Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder. |
| [getTopInch()](#getTopInch--) | Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder. |
| [getTopToCorner()](#getTopToCorner--) | Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Şeklin sol üst köşe sütunundan yatay ofsetini alır. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Şeklin sol üst köşe satırından dikey ofsetini alır. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Sol üst köşe sütun indeksini temsil eder. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Üst sol köşe satır indeksini temsil eder. |
| [getWidth()](#getWidth--) | Şeklin genişliğini piksel biriminde temsil eder. |
| [getWidthCM()](#getWidthCM--) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [getWidthInch()](#getWidthInch--) | Şeklin genişliğini inç biriminde temsil eder. |
| [getWidthPt()](#getWidthPt--) | Şeklin genişliğini puan biriminde temsil eder. |
| [getWidthScale()](#getWidthScale--) | Orijinal resim genişliğinin yüzde biriminde genişlik ölçeğini alır. |
| [getX()](#getX--) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde alır. |
| [getY()](#getY--) | Şeklin çalışma sayfası üst kenarından dikey ofsetini piksel biriminde alır. |
| [getZOrderPosition()](#getZOrderPosition--) | Bir şeklin z-sırasındaki konumunu döndürür. |
| [hasLine()](#hasLine--) | Şeklin çizgi kenarlığının görünür olup olmadığını alır. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Şeklin dikey olarak çevrilip çevrilmediğini alır. |
| [isGroup()](#isGroup--) | Şeklin bir grup olup olmadığını gösterir. |
| [isHidden()](#isHidden--) | Nesnenin görünür olup olmadığını gösterir. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True, en boy oranı değişikliklerine izin verilmediği anlamına gelir. |
| [isLocked()](#isLocked--) | Nesne kilitliyse True, sayfa korunduğunda nesne değiştirilebiliyorsa False. |
| [isTextWrapped()](#isTextWrapped--) | Metin içeren şeklin metin kaydırma türünü alır. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Resmi belirtilen konuma taşır. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Şekli belirtilen bir aralığa taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Şeklin hiperlinkini kaldırın. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Görüntüyü oluşturur ve bir akışa kaydeder. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Bir [GridShape](../../com.aspose.gridweb/gridshape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Bir resmin kenar çizgisinin [Color](../../com.aspose.cells/color) değerini temsil eder. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Resmin kenar çizgisinin kalınlığını pt biriminde ayarlar. |
| [setBottom(int value)](#setBottom-int-) | Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [setData(byte[] value)](#setData-byte---) | Resmin verisini alır. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Şeklin dikey olarak çevrilip çevrilmediğini ayarlar. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Şeklin çizgi kenarlığının görünür olup olduğunu ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Şeklin yüksekliğini piksel biriminde temsil eder. |
| [setHeightCM(double value)](#setHeightCM-double-) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [setHeightInch(double value)](#setHeightInch-double-) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [setHeightPt(double value)](#setHeightPt-double-) | Şeklin yüksekliğini puan biriminde temsil eder. |
| [setHeightScale(int value)](#setHeightScale-int-) | Yükseklik ölçeğini, orijinal resim yüksekliğinin yüzde birimi olarak ayarlar. |
| [setHidden(boolean value)](#setHidden-boolean-) | Nesnenin görünür olup olmadığını gösterir. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Bu metin kutusundaki veri ve bazı biçimlendirmeleri içeren html dizesini ayarlar. |
| [setID(String value)](#setID-java.lang.String-) | Resmin kimliğini alır / ayarlar. |
| [setLeft(int value)](#setLeft-int-) | Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder. |
| [setLeftCM(double value)](#setLeftCM-double-) | Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder. |
| [setLeftInch(double value)](#setLeftInch-double-) | Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Denetimin değerine bağlı çalışma sayfası aralığını ayarlar. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True, en boy oranı değişikliklerine izin verilmediği anlamına gelir. |
| [setLocked(boolean value)](#setLocked-boolean-) | Nesne kilitliyse True, sayfa korunduğunda nesne değiştirilebiliyorsa False. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Şeklin sağ alt köşe sütunundan yatay ofsetini ayarlar. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Şeklin sağ alt köşe satırından dikey ofsetini ayarlar. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Sağ alt köşe sütun indeksini temsil eder. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Sağ alt köşe satır indeksini temsil eder. |
| [setName(String value)](#setName-java.lang.String-) | Şeklin adını ayarlar. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir. |
| [setRight(int value)](#setRight-int-) | Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Şeklin dönüşünü ayarlar. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Bağlantılı görüntünün kaynak dosyasının yolunu ve adını ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Bu TextBox nesnesindeki dizeyi temsil eder. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Metin içeren şeklin metin sarma türünü ayarlar. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Mevcut şekil nesnesinin başlığını (altyazısını) belirtir. |
| [setTop(int value)](#setTop-int-) | Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| [setTopCM(double value)](#setTopCM-double-) | Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder. |
| [setTopInch(double value)](#setTopInch-double-) | Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Şeklin üst sol köşe sütunundan yatay kaydırmasını ayarlar. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Şeklin üst sol köşe satırından dikey kaydırmasını ayarlar. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Sol üst köşe sütun indeksini temsil eder. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Üst sol köşe satır indeksini temsil eder. |
| [setWidth(int value)](#setWidth-int-) | Şeklin genişliğini piksel biriminde temsil eder. |
| [setWidthCM(double value)](#setWidthCM-double-) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [setWidthInch(double value)](#setWidthInch-double-) | Şeklin genişliğini inç biriminde temsil eder. |
| [setWidthPt(double value)](#setWidthPt-double-) | Şeklin genişliğini puan biriminde temsil eder. |
| [setWidthScale(int value)](#setWidthScale-int-) | Genişlik ölçeğini, orijinal resim genişliğinin yüzde biriminde ayarlar. |
| [setX(int value)](#setX-int-) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini piksel biriminde ayarlar. |
| [setY(int value)](#setY-int-) | Şeklin çalışma sayfası üst kenarından dikey kaydırmasını, piksel biriminde ayarlar. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Bir şeklin z-sırasındaki konumunu döndürür. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Şekle bir hiperlink ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Resmi sağ üst köşeye taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | satır indeksi. |
| rightColumn | int | sütun indeksi. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Bir [GridShape](../../com.aspose.gridweb/gridshape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Bir resmin kenar çizgisinin [Color](../../com.aspose.cells/color) değerini temsil eder.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Bir resmin kenar çizgisinin kalınlığını pt biriminde alır.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Resmin verisini alır.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Şeklin yüksekliğini piksel biriminde temsil eder.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Şeklin yüksekliğini inç biriminde temsil eder.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Şeklin yüksekliğini inç biriminde temsil eder.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Şeklin yüksekliğini puan biriminde temsil eder.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Orijinal resim yüksekliğinin yüzde birimi olarak yükseklik ölçeğini alır. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Bu metin kutusunda veri ve bazı biçimlendirmeleri içeren html dizesini alır.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Şeklin köprü bağlantısını alır.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Resmin kimliğini alır / ayarlar.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Resmin görüntü formatını alır.

Bakın [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Denetimin değerine bağlı çalışma sayfası aralığını alır.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Şeklin sağ alt köşe sütunundan yatay ofsetini alır. Değer aralığı 0 ile 1024 arasındadır.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Şeklin sağ alt köşe satırından dikey ofsetini alır. Değer aralığı 0 ile 256 arasındadır.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Sağ alt köşe sütun indeksini temsil eder.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Sağ alt köşe satır indeksini temsil eder.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Şeklin adını alır.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Resmin orijinal yüksekliğini alır.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Resmin orijinal yüksekliğini santimetre biriminde alır.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Resmin orijinal yüksekliğini, inç biriminde alır.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Resmin orijinal genişliğini alır.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Resmin orijinal genişliğini, santimetre biriminde alır.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Resmin orijinal genişliğini, inç biriminde alır.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Şeklin dönüşünü alır.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Bağlantılı görüntünün kaynak dosyasının yolunu ve adını alır.

**Remarks**

Varsayılan değer boş bir dizedir. SourceFullName boş bir dize değilse, görüntü bağlıdır. SourceFullName boş bir dize değilse ancak Data null ise, görüntü bağlıdır ve dosyada depolanmaz.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Bu TextBox nesnesindeki dizeyi temsil eder.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Mevcut şekil nesnesinin başlığını (altyazısını) belirtir.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder.

**Remarks**

Şekil grafikte ise, şeklin üst kenarından dikey ofsetini temsil eder.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Şeklin sol üst köşe sütunundan yatay ofsetini alır. Değer aralığı 0 ile 1024 arasındadır.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Şeklin sol üst köşe satırından dikey ofsetini alır. Değer aralığı 0 ile 256 arasındadır.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Sol üst köşe sütun indeksini temsil eder.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Üst sol köşe satır indeksini temsil eder.

**Remarks**

Şekil bir şekil içinde veya bir grup içinde ise, UpperLeftRow yoksayılacaktır.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Şeklin genişliğini piksel biriminde temsil eder.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Şeklin genişliğini santimetre biriminde temsil eder.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Şeklin genişliğini inç biriminde temsil eder.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Şeklin genişliğini puan biriminde temsil eder.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Orijinal resim genişliğinin yüzde birimi olarak genişlik ölçeğini alır. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde alır.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Şeklin çalışma sayfası üst kenarından dikey ofsetini piksel biriminde alır.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Bir şeklin z-sırasındaki konumunu döndürür.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Şeklin çizgi kenarlığının görünür olup olmadığını alır.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Şeklin dikey olarak çevrilip çevrilmediğini alır.

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Şeklin bir grup olup olmadığını gösterir.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Nesnenin görünür olup olmadığını gösterir.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True, en boy oranı değişikliklerine izin verilmediği anlamına gelir.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Nesne kilitliyse True, sayfa korunduğunda nesne değiştirilebiliyorsa False.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Metin içeren şeklin metin kaydırma türünü alır.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Resmi belirtilen konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| upperLeftRow | int | Üst sol satır indeksi. |
| upperLeftColumn | int | Üst sol sütun indeksi. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Şekli belirtilen bir aralığa taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| upperLeftRow | int | Üst sol satır indeksi. |
| upperLeftColumn | int | Üst sol sütun indeksi. |
| lowerRightRow | int | Alt sağ satır indeksi |
| lowerRightColumn | int | Alt sağ sütun indeksi |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Şeklin hiperlinkini kaldırın.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Görüntüyü oluşturur ve bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Bir [GridShape](../../com.aspose.gridweb/gridshape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Bir resmin kenar çizgisinin [Color](../../com.aspose.cells/color) değerini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Resmin kenar çizgisinin kalınlığını pt biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Resmin verisini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Şeklin dikey olarak çevrilip çevrilmediğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Şeklin çizgi kenarlığının görünür olup olduğunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Şeklin yüksekliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Şeklin yüksekliğini inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Şeklin yüksekliğini inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Şeklin yüksekliğini puan biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Yükseklik ölçeğini, orijinal resim yüksekliğinin yüzde birimi olarak ayarlar. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Nesnenin görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Bu metin kutusundaki veri ve bazı biçimlendirmeleri içeren html dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Resmin kimliğini alır / ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Denetimin değerine bağlı çalışma sayfası aralığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True, en boy oranı değişikliklerine izin verilmediği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Nesne kilitliyse True, sayfa korunduğunda nesne değiştirilebiliyorsa False.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Şeklin sağ alt köşe sütunundan yatay ofsetini ayarlar. Değer aralığı 0 ile 1024 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Şeklin sağ alt köşe satırından dikey ofsetini ayarlar. Değer aralığı 0 ile 256 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Sağ alt köşe sütun indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Sağ alt köşe satır indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Şeklin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Şeklin dönüşünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Bağlantılı görüntünün kaynak dosyasının yolunu ve adını ayarlar.

**Remarks**

Varsayılan değer boş bir dizedir. SourceFullName boş bir dize değilse, görüntü bağlıdır. SourceFullName boş bir dize değilse ancak Data null ise, görüntü bağlıdır ve dosyada depolanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Bu TextBox nesnesindeki dizeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Metin içeren şeklin metin sarma türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Mevcut şekil nesnesinin başlığını (altyazısını) belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder.

**Remarks**

Şekil grafikte ise, şeklin üst kenarından dikey ofsetini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Şeklin sol üst köşe sütunundan yatay ofsetini ayarlar. Değer aralığı 0 ile 1024 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Şeklin sol üst köşe satırından dikey ofsetini ayarlar. Değer aralığı 0 ile 256 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Sol üst köşe sütun indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Üst sol köşe satır indeksini temsil eder.

**Remarks**

Şekil bir şekil içinde veya bir grup içinde ise, UpperLeftRow yoksayılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Şeklin genişliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Şeklin genişliğini santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Şeklin genişliğini inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Şeklin genişliğini puan biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Genişlik ölçeğini, orijinal resim genişliğinin yüzde birimi olarak ayarlar. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Şeklin çalışma sayfası üst kenarından dikey kaydırmasını, piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Bir şeklin z-sırasındaki konumunu döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

