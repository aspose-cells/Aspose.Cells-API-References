---
title: "SmartArtShape"
second_title: "Aspose.Cells for Java API Referansı"
description: "Smart art'ı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/smartartshape/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class SmartArtShape extends Shape
```

Smart art'ı temsil eder.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook("YourFile.xlsx");
 
         //Gets a SmartArt shape.
         Shape shape = null;
         ShapeCollection shapes = book.getWorksheets().get(0).getShapes();
         for(Shape s : (Iterable<Shape>) shapes)
         {
             if(s.getMsoDrawingType() == com.aspose.cells.MsoDrawingType.SMART_ART)
             {
                 //is SmartArt Shape
                 //do what you want
                 break;
             }
         }
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Şekle bir hiperlink ekler. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Resmi sağ üst köşeye taşır. |
| [calculateTextSize()](#calculateTextSize--) | Metin alanını yeniden hesapla |
| [characters(int startIndex, int length)](#characters-int-int-) | Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Tüm metin içeriğini gösterecek şekilde bir metin alanını yeniden hesapla. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Bazı karakterleri yazı tipi ayarıyla biçimlendirir. |
| [getActiveXControl()](#getActiveXControl--) | ActiveX kontrolünü alır. |
| [getActualBox()](#getActualBox--) | Şeklin gerçek konumunu ve boyutunu al (dönme, çevirme vb. uygulandıktan sonra). |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Gerçek alt satırı al. |
| [getAlternativeText()](#getAlternativeText--) | [Shape](../../com.aspose.cells/shape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [getAnchorType()](#getAnchorType--) | Şekil çapa yer tutucusunun tipini alır. |
| [getAutoShapeType()](#getAutoShapeType--) | Otomatik şekil tipini alır. |
| [getBottom()](#getBottom--) | Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [getCharacters()](#getCharacters--) | Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Bağlantı noktalarını al. |
| [getControlData()](#getControlData--) | Denetimin verilerini alır. |
| [getCreateId()](#getCreateId--) | Bu şekil için oluşturma kimliğini alır. |
| [getFill()](#getFill--) | Belirtilen şekil için doldurma biçimlendirme özelliklerini içeren bir [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) nesnesi döndürür. |
| [getFillFormat()](#getFillFormat--) | Belirtilen şekil için doldurma biçimlendirme özelliklerini içeren bir MsoFillFormat nesnesi döndürür. |
| [getFont()](#getFont--) | Şeklin yazı tipini temsil eder. |
| [getFormatPicture()](#getFormatPicture--) | Resim formatının seçeneklerini alır. |
| [getGeometry()](#getGeometry--) | Geometriyi alır |
| [getGlow()](#getGlow--) | Grafik öğesi veya şekil için parıltı etkisini belirten bir [GlowEffect](../../com.aspose.cells/gloweffect) nesnesini temsil eder. |
| [getGroup()](#getGroup--) | Bu şekli içeren grup şekli alır. |
| [getHeight()](#getHeight--) | Şeklin yüksekliğini piksel biriminde temsil eder. |
| [getHeightCM()](#getHeightCM--) | Şeklin yüksekliğini santimetre biriminde temsil eder. |
| [getHeightInShape()](#getHeightInShape--) | Şeklin, üst ana şeklin kenarından dikey ofsetini, ana şeklin yüksekliğinin 1/4000 birimi olarak temsil eder. |
| [getHeightInch()](#getHeightInch--) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [getHeightPt()](#getHeightPt--) | Şeklin yüksekliğini puan biriminde temsil eder. |
| [getHeightScale()](#getHeightScale--) | Orijinal resim yüksekliğinin yüzde biriminde yükseklik ölçeğini alır. |
| [getHtmlText()](#getHtmlText--) | Bu metin kutusunda veri ve bazı biçimleri içeren html dizesini alır. |
| [getHyperlink()](#getHyperlink--) | Şeklin köprü bağlantısını alır. |
| [getId()](#getId--) | Bu şeklin tanımlayıcısını alır. |
| [getInputRange()](#getInputRange--) | Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Denetimi doldurmak için kullanılan aralığı alır. |
| [getLeft()](#getLeft--) | Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder. |
| [getLeftCM()](#getLeftCM--) | Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder. |
| [getLeftInShape()](#getLeftInShape--) | Şeklin üst şeklin sol kenarından yatay kaymasını, üst şeklin genişliğinin 1/4000'i biriminde temsil eder. |
| [getLeftInch()](#getLeftInch--) | Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder. |
| [getLeftToCorner()](#getLeftToCorner--) | Şeklin çalışma sayfasının sol kenarından yatay kaymasını alır. |
| [getLine()](#getLine--) | Çizgi stilini alır |
| [getLineFormat()](#getLineFormat--) | Belirtilen şekil için çizgi biçimlendirme özelliklerini içeren bir MsoLineFormat nesnesi döndürür. |
| [getLinkedCell()](#getLinkedCell--) | Denetimin değerine bağlı çalışma sayfası aralığını alır. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Denetimin değerine bağlı aralığı alır. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Kilitli özelliğinin değerini alır. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Şeklin sağ alt köşe sütunundan yatay kaymasını alır. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Şeklin sağ alt köşe satırından dikey kaymasını alır. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Sağ alt köşe sütun indeksini temsil eder. |
| [getLowerRightRow()](#getLowerRightRow--) | Sağ alt köşe satır indeksini temsil eder. |
| [getMacroName()](#getMacroName--) | Makronun adını alır. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Çizim tipini alır. |
| [getName()](#getName--) | Şeklin adını alır. |
| [getPaths()](#getPaths--) | Özel geometrik şeklin yollarını alır. |
| [getPlacement()](#getPlacement--) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [getReflection()](#getReflection--) | Grafik öğesi veya şekil için yansıma etkisini belirten bir [ReflectionEffect](../../com.aspose.cells/reflectioneffect) nesnesini temsil eder. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Akıllı sanatı gruplanmış şekillere dönüştürme. |
| [getRichFormattings()](#getRichFormattings--) | Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [getRight()](#getRight--) | Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder. |
| [getRotationAngle()](#getRotationAngle--) | Şeklin dönüşünü alır. |
| [getShadowEffect()](#getShadowEffect--) | Grafik öğesi veya şekil için gölge etkisini belirten bir [ShadowEffect](../../com.aspose.cells/shadoweffect) nesnesini temsil eder. |
| [getSoftEdges()](#getSoftEdges--) | Kenarlar için uygulanacak bulanıklık yarıçapını, nokta biriminde alır. |
| [getSpid()](#getSpid--) | Uygulamanın belirli şekli tanımlamak için kullanabileceği isteğe bağlı bir dize tanımlayıcısını belirtir. |
| [getSpt()](#getSpt--) | Uygulamanın belirli şekli tanımlı bir şekil türüyle ilişkilendirmek için kullanabileceği isteğe bağlı bir sayıyı belirtir. |
| [getText()](#getText--) | Bu şeklin metnini alır. |
| [getTextBody()](#getTextBody--) | Şeklin metin ayarını alır. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Şekildeki metin bilgisini alır |
| [getTextDirection()](#getTextDirection--) | Bu nesne için metin akış yönünü alır. |
| [getTextEffect()](#getTextEffect--) | Belirtilen şekil için metin-etkisi biçimlendirme özelliklerini içeren bir TextEffectFormat nesnesi döndürür. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Şeklin metin yatay hizalama türünü alır. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Metin içeren şeklin metin yatay taşma türünü alır. |
| [getTextOptions()](#getTextOptions--) | Şeklin metin seçeneklerini temsil eder. |
| [getTextOrientationType()](#getTextOrientationType--) | Şeklin metin yönlendirme türünü alır. |
| [getTextShapeType()](#getTextShapeType--) | Önceden ayarlanmış metin şekil türünü alır. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Şeklin metin dikey hizalama türünü alır. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Metin içeren şeklin metin dikey taşma türünü alır. |
| [getThreeDFormat()](#getThreeDFormat--) | Şeklin 3D biçimini alır. |
| [getTitle()](#getTitle--) | Mevcut şekil nesnesinin başlığını (altyazısını) belirtir. |
| [getTop()](#getTop--) | Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| [getTopCM()](#getTopCM--) | Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder. |
| [getTopInShape()](#getTopInShape--) | Şeklin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000'i biriminde dikey ofsetini temsil eder. |
| [getTopInch()](#getTopInch--) | Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder. |
| [getTopToCorner()](#getTopToCorner--) | Şeklin çalışma sayfası üst kenarından dikey ofsetini, piksel biriminde alır. |
| [getType()](#getType--) | Otomatik şekil tipini alır. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Şeklin sol üst köşe sütunundan yatay ofsetini alır. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Şeklin sol üst köşe satırından dikey ofsetini alır. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Sol üst köşe sütun indeksini temsil eder. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Üst satır indeksini temsil eder. |
| [getWidth()](#getWidth--) | Şeklin genişliğini piksel biriminde temsil eder. |
| [getWidthCM()](#getWidthCM--) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [getWidthInShape()](#getWidthInShape--) | Şeklin genişliğini, üst şeklin 1/4000'i biriminde temsil eder. |
| [getWidthInch()](#getWidthInch--) | Şeklin genişliğini inç biriminde temsil eder. |
| [getWidthPt()](#getWidthPt--) | Şeklin genişliğini puan biriminde temsil eder. |
| [getWidthScale()](#getWidthScale--) | Orijinal resim genişliğinin yüzde biriminde genişlik ölçeğini alır. |
| [getWorksheet()](#getWorksheet--) | Bu şekli içeren [Worksheet](../../com.aspose.cells/worksheet) nesnesini alır. |
| [getX()](#getX--) | Şeklin çalışma sayfası sol kenarından yatay ofsetini piksel biriminde alır. |
| [getY()](#getY--) | Şeklin çalışma sayfası üst kenarından dikey ofsetini piksel biriminde alır. |
| [getZOrderPosition()](#getZOrderPosition--) | Bir şeklin z-sırasındaki konumunu döndürür. |
| [hasLine()](#hasLine--) | Şeklin çizgi kenarlığının görünür olup olmadığını alır. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir. |
| [isDecorative()](#isDecorative--) | Nesnenin dekoratif olup olmadığını gösterir. |
| [isEquation()](#isEquation--) | Şeklin yalnızca bir denklem içerip içermediğini gösterir. |
| [isFilled()](#isFilled--) | Dolgu biçiminin görünür olup olmadığını gösterir. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Şeklin yatay olarak çevrilip çevrilmediğini alır. |
| [isFlippedVertically()](#isFlippedVertically--) | Şeklin dikey olarak çevrilip çevrilmediğini alır. |
| [isGroup()](#isGroup--) | Bu şeklin bir grup şekli olup olmadığını gösterir. |
| [isHidden()](#isHidden--) | Nesnenin görünür olup olmadığını gösterir. |
| [isInGroup()](#isInGroup--) | Şeklin gruplanıp gruplanmadığını gösterir. |
| [isLockAspectRatio()](#isLockAspectRatio--) | Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir. |
| [isLocked()](#isLocked--) | Doğru, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. |
| [isPrintable()](#isPrintable--) | Nesnenin yazdırılabilir olup olmadığını gösterir. |
| [isRichText()](#isRichText--) | Metnin zengin metin olup olmadığı. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Şeklin aynı olup olmadığını döndürür. |
| [isSmartArt()](#isSmartArt--) | Şeklin akıllı sanat olup olmadığını gösterir. |
| [isTextWrapped()](#isTextWrapped--) | Metin içeren şeklin metin kaydırma türünü alır. |
| [isWordArt()](#isWordArt--) | Bu şeklin kelime sanatı olup olmadığını gösterir. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Şekli belirtilen bir aralığa taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | ActiveX denetimini kaldır. |
| [removeHyperlink()](#removeHyperlink--) | Şeklin köprü bağlantısını kaldırır. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | [Shape](../../com.aspose.cells/shape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [setAnchorType(int value)](#setAnchorType-int-) | Şekil çapa yer tutucusunun türünü ayarlar. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Otomatik şekil türünü ayarlar. |
| [setBottom(int value)](#setBottom-int-) | Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Bu şekil için oluşturma kimliğini ayarlar. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Nesnenin dekoratif olup olmadığını gösterir. |
| [setFilled(boolean value)](#setFilled-boolean-) | Dolgu biçiminin görünür olup olmadığını gösterir. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Şeklin yatay olarak çevrilip çevrilmediğini ayarlar. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Şeklin dikey olarak çevrilip çevrilmediğini ayarlar. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Şeklin yazı tipini temsil eder. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Şeklin çizgi kenarlığının görünür olup olduğunu ayarlar. |
| [setHeight(int value)](#setHeight-int-) | Şeklin yüksekliğini piksel biriminde temsil eder. |
| [setHeightCM(double value)](#setHeightCM-double-) | Şeklin yüksekliğini santimetre biriminde temsil eder. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Şeklin, üst ana şeklin kenarından dikey ofsetini, ana şeklin yüksekliğinin 1/4000 birimi olarak temsil eder. |
| [setHeightInch(double value)](#setHeightInch-double-) | Şeklin yüksekliğini inç biriminde temsil eder. |
| [setHeightPt(double value)](#setHeightPt-double-) | Şeklin yüksekliğini puan biriminde temsil eder. |
| [setHeightScale(int value)](#setHeightScale-int-) | Yükseklik ölçeğini, orijinal resim yüksekliğinin yüzde birimi olarak ayarlar. |
| [setHidden(boolean value)](#setHidden-boolean-) | Nesnenin görünür olup olmadığını gösterir. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Bu metin kutusunda veri ve bazı biçimleri içeren HTML dizesini ayarlar. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını ayarlar. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Denetimi doldurmak için kullanılan aralığı ayarlar. |
| [setLeft(int value)](#setLeft-int-) | Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder. |
| [setLeftCM(double value)](#setLeftCM-double-) | Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Şeklin üst şeklin sol kenarından yatay kaymasını, üst şeklin genişliğinin 1/4000'i biriminde temsil eder. |
| [setLeftInch(double value)](#setLeftInch-double-) | Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Şeklin çalışma sayfası sol kenarından yatay ofsetini ayarlar. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Denetimin değerine bağlı çalışma sayfası aralığını ayarlar. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Denetimin değerine bağlı aralığı ayarlar. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir. |
| [setLocked(boolean value)](#setLocked-boolean-) | Doğru, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Kilitli özelliği ayarla. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Şeklin sağ alt köşe sütunundan yatay ofsetini ayarlar. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Şeklin sağ alt köşe satırından dikey ofsetini ayarlar. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Sağ alt köşe sütun indeksini temsil eder. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Sağ alt köşe satır indeksini temsil eder. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Makronun adını ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Şeklin adını ayarlar. |
| [setPlacement(int value)](#setPlacement-int-) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Nesnenin yazdırılabilir olup olmadığını gösterir. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir. |
| [setRight(int value)](#setRight-int-) | Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Şeklin dönüşünü ayarlar. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Kenarlara uygulanacak bulanıklık yarıçapını, nokta biriminde ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Bu şeklin metnini ayarlar. |
| [setTextDirection(int value)](#setTextDirection-int-) | Bu nesne için metin akış yönünü ayarlar. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Şeklin metin yatay hizalama türünü ayarlar. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Metin içeren şeklin metin yatay taşma türünü ayarlar. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Şeklin metin seçeneklerini temsil eder. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Şeklin metin yönlendirme türünü ayarlar. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Önceden ayarlanmış metin şekli türünü ayarlar. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Şeklin metin dikey hizalama türünü ayarlar. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Metin içeren şeklin metin dikey taşma türünü ayarlar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Metin içeren şeklin metin sarma türünü ayarlar. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Mevcut şekil nesnesinin başlığını (altyazısını) belirtir. |
| [setTop(int value)](#setTop-int-) | Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| [setTopCM(double value)](#setTopCM-double-) | Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder. |
| [setTopInShape(int value)](#setTopInShape-int-) | Şeklin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000'i biriminde dikey ofsetini temsil eder. |
| [setTopInch(double value)](#setTopInch-double-) | Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Şeklin çalışma sayfası üst kenarından dikey kaydırmasını, piksel biriminde ayarlar. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Şeklin üst sol köşe sütunundan yatay kaydırmasını ayarlar. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Şeklin üst sol köşe satırından dikey kaydırmasını ayarlar. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Sol üst köşe sütun indeksini temsil eder. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Üst satır indeksini temsil eder. |
| [setWidth(int value)](#setWidth-int-) | Şeklin genişliğini piksel biriminde temsil eder. |
| [setWidthCM(double value)](#setWidthCM-double-) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Şeklin genişliğini, üst şeklin 1/4000'i biriminde temsil eder. |
| [setWidthInch(double value)](#setWidthInch-double-) | Şeklin genişliğini inç biriminde temsil eder. |
| [setWidthPt(double value)](#setWidthPt-double-) | Şeklin genişliğini puan biriminde temsil eder. |
| [setWidthScale(int value)](#setWidthScale-int-) | Genişlik ölçeğini, orijinal resim genişliğinin yüzde biriminde ayarlar. |
| [setX(int value)](#setX-int-) | Şeklin çalışma sayfası sol kenarından yatay kaydırmasını, piksel biriminde ayarlar. |
| [setY(int value)](#setY-int-) | Şeklin çalışma sayfası üst kenarından dikey kaydırmasını, piksel biriminde ayarlar. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Bir şeklin z-sırasındaki konumunu döndürür. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Şekli öne getirir veya arkaya gönderir. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Şekil görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Şekli bir akışa kaydeder. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Şekli bir dosyaya kaydeder. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Seçili değeri, bağlı hücrenin değeriyle günceller. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Şekle bir hiperlink ekler.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Resmi sağ üst köşeye taşır.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | satır indeksi. |
| rightColumn | int | sütun indeksi. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Metin alanını yeniden hesapla

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Metnin Boyutu bir dizi içinde (genişlik ve yükseklik).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

**Remarks**

Bu yöntem yalnızca başlıklı şekil üzerinde çalışır.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Karakterin başlangıç indeksi. |
| length | int | Karakter sayısı. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Tüm metin içeriğini gösterecek şekilde bir metin alanını yeniden hesapla.

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Bazı karakterleri yazı tipi ayarıyla biçimlendirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| length | int | Uzunluk. |
| font | [Font](../../com.aspose.cells/font) | Yazı tipi ayarı. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Yazı tipi ayarının bayrağı. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


ActiveX kontrolünü alır.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


Şeklin gerçek konumunu ve boyutunu al (dönme, çevirme vb. uygulandıktan sonra).

**Remarks**

Not:Arayüz tam olarak işlevsel değildir, özellikle konum bilgisi doğru değildir. İşlev tamamlanana kadar bu arayüzün kullanılmaması önerilir.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Pozisyon ve boyutu x, y, w, h sırasıyla döndürür.
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Gerçek alt satırı al.

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


[Shape](../../com.aspose.cells/shape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


Şekil çapa yer tutucusunun tipini alır.

Bakınız [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


Otomatik şekil tipini alır.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder.

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.GetRichFormattings() yöntemini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Tüm Karakter nesneleri
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Bağlantı noktalarını al.

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - Bağlantı noktasının [X,Y] çiftleri. Her öğe bir float[2] dizisidir, [0] x'i ve [1] y'yi temsil eder.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Denetimin verilerini alır.

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


Bu şekil için oluşturma kimliğini alır.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Belirtilen şekil için doldurma biçimlendirme özelliklerini içeren bir [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) nesnesi döndürür.

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


Belirtilen şekil için doldurma biçimlendirme özelliklerini içeren bir MsoFillFormat nesnesi döndürür.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.Fill özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Şeklin yazı tipini temsil eder.

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


Resim formatının seçeneklerini alır.

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Geometriyi alır

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


Grafik öğesi veya şekil için parıltı etkisini belirten bir [GlowEffect](../../com.aspose.cells/gloweffect) nesnesini temsil eder.

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


Bu şekli içeren grup şekli alır.

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Şeklin yüksekliğini piksel biriminde temsil eder.

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Şeklin yüksekliğini santimetre biriminde temsil eder.

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


Şeklin, üst ana şeklin kenarından dikey ofsetini, ana şeklin yüksekliğinin 1/4000 birimi olarak temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Şeklin yüksekliğini inç biriminde temsil eder.

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Şeklin yüksekliğini puan biriminde temsil eder.

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Orijinal resim yüksekliğinin yüzde birimi olarak yükseklik ölçeğini alır. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür;

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Bu metin kutusunda veri ve bazı biçimleri içeren html dizesini alır.

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


Şeklin köprü bağlantısını alır.

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


Bu şeklin tanımlayıcısını alır.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır.

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


Denetimi doldurmak için kullanılan aralığı alır.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Kontrolü doldurmak için kullanılan aralık.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder.

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Şeklin sol sütunundan yatay kaymasını, santimetre biriminde temsil eder.

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


Şeklin üst şeklin sol kenarından yatay kaymasını, üst şeklin genişliğinin 1/4000'i biriminde temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Şeklin sol sütunundan yatay kaymasını, inç biriminde temsil eder.

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Şeklin çalışma sayfasının sol kenarından yatay kaymasını alır.

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


Çizgi stilini alır

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


Belirtilen şekil için çizgi biçimlendirme özelliklerini içeren bir MsoLineFormat nesnesi döndürür.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.Line özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Denetimin değerine bağlı çalışma sayfası aralığını alır.

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


Denetimin değerine bağlı aralığı alır.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Kontrolün değerine bağlı aralık.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Kilitli özelliğinin değerini alır.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Şeklin kilitli özelliğinin türü. |

**Returns:**
boolean - Kilitli özelliğin değerini döndürür.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Şeklin sağ alt köşe sütunundan yatay kaymasını alır.

**Remarks**

Değer aralığı 0 ile 1024 arasındadır.

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Şeklin sağ alt köşe satırından dikey kaymasını alır.

**Remarks**

Değer aralığı 0 ile 256 arasındadır.

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Sağ alt köşe sütun indeksini temsil eder.

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Sağ alt köşe satır indeksini temsil eder.

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


Makronun adını alır.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Çizim tipini alır.

Bakınız [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Şeklin adını alır.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Özel geometrik şeklin yollarını alır.

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Grafik öğesi veya şekil için yansıma etkisini belirten bir [ReflectionEffect](../../com.aspose.cells/reflectioneffect) nesnesini temsil eder.

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir.

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


Akıllı sanatı gruplanmış şekillere dönüştürme.

**Example**

```
         GroupShape groupShape = shape.getResultOfSmartArt();
         if(groupShape != null)
         {
             //do what you want
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tüm Karakter nesneleri
### getRight() {#getRight--}
```
public int getRight()
```


Şeklin sağ alt köşe sütunundan yatay kaymasının genişliğini, piksel biriminde temsil eder.

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Şeklin dönüşünü alır.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Grafik öğesi veya şekil için gölge etkisini belirten bir [ShadowEffect](../../com.aspose.cells/shadoweffect) nesnesini temsil eder.

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


Kenarlar için uygulanacak bulanıklık yarıçapını, nokta biriminde alır.

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


Uygulamanın belirli şekli tanımlamak için kullanabileceği isteğe bağlı bir dize tanımlayıcısını belirtir.

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


Uygulamanın belirli şekli tanımlı bir şekil türüyle ilişkilendirmek için kullanabileceği isteğe bağlı bir sayıyı belirtir.

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Bu şeklin metnini alır.

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


Şeklin metin ayarını alır.

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


Şekildeki metin bilgisini alır

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Bu nesne için metin akış yönünü alır.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


Belirtilen şekil için metin-efekti biçimlendirme özelliklerini içeren bir TextEffectFormat nesnesi döndürür. WordArt temsil eden Shape nesnelerine uygulanır.

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Şeklin metin yatay hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Metin içeren şeklin metin yatay taşma türünü alır.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Şeklin metin seçeneklerini temsil eder.

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


Şeklin metin yönlendirme türünü alır.

Bakınız [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Önceden ayarlanmış metin şekil türünü alır.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Şeklin metin dikey hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Metin içeren şeklin metin dikey taşma türünü alır.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


Şeklin 3D biçimini alır.

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


Mevcut şekil nesnesinin başlığını (altyazısını) belirtir.

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder.

**Remarks**

Şekil grafikte ise, şeklin üst kenarından dikey ofsetini temsil eder.

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Şeklin üst satırından dikey ofsetini, santimetre biriminde temsil eder.

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


Şeklin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000'i biriminde dikey ofsetini temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Şeklin üst satırından dikey ofsetini, inç biriminde temsil eder.

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Şeklin çalışma sayfası üst kenarından dikey ofsetini, piksel biriminde alır.

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Otomatik şekil tipini alır.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Şeklin sol üst köşe sütunundan yatay ofsetini alır.

**Remarks**

Değer aralığı 0 ile 1024 arasındadır.

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Şeklin sol üst köşe satırından dikey ofsetini alır.

**Remarks**

Değer aralığı 0 ile 256 arasındadır.

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Sol üst köşe sütun indeksini temsil eder.

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Üst satır indeksini temsil eder.

**Remarks**

Şekil bir şekil içinde veya bir grup içinde ise, UpperLeftRow yoksayılacaktır.

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Şeklin genişliğini piksel biriminde temsil eder.

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Şeklin genişliğini santimetre biriminde temsil eder.

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


Şeklin genişliğini, üst şeklin 1/4000'i biriminde temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Şeklin genişliğini inç biriminde temsil eder.

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Şeklin genişliğini puan biriminde temsil eder.

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Orijinal resim genişliğinin yüzde birimi olarak genişlik ölçeğini alır. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür;

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Bu şekli içeren [Worksheet](../../com.aspose.cells/worksheet) nesnesini alır.

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


Şeklin çalışma sayfası sol kenarından yatay ofsetini piksel biriminde alır.

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Şeklin çalışma sayfası üst kenarından dikey ofsetini piksel biriminde alır.

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Bir şeklin z-sırasındaki konumunu döndürür.

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Şeklin çizgi kenarlığının görünür olup olmadığını alır.

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir.

**Remarks**

Yalnızca resimler ve Ole Nesneleri için.

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


Nesnenin dekoratif olup olmadığını gösterir.

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Şeklin yalnızca bir denklem içerip içermediğini gösterir.

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


Dolgu biçiminin görünür olup olmadığını gösterir.

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


Şeklin yatay olarak çevrilip çevrilmediğini alır.

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Şeklin dikey olarak çevrilip çevrilmediğini alır.

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Bu şeklin bir grup şekli olup olmadığını gösterir.

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Nesnenin görünür olup olmadığını gösterir.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Şeklin gruplanıp gruplanmadığını gösterir.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir.

**Remarks**

Yalnızca resimler ve Ole Nesneleri için. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.IsAspectRatioLocked özelliğini kullanın. Bu özellik Temmuz 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya çalışma sayfasındaki nesneler korunduğunda anlamlı olduğunu unutmayın.

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Nesnenin yazdırılabilir olup olmadığını gösterir. False ise, bu şekil yazdırma sırasında basılmaz.

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Metnin zengin metin olup olmadığı.

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


Şeklin aynı olup olmadığını döndürür.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Şeklin akıllı sanat olup olmadığını gösterir.

**Remarks**

Yalnızca ooxml dosyası için.

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Metin içeren şeklin metin kaydırma türünü alır.

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


Bu şeklin kelime sanatı olup olmadığını gösterir.

**Remarks**

Yalnızca xls dosyasının Eski Şekli için.

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Şekli belirtilen bir aralığa taşır.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


ActiveX denetimini kaldır.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Şeklin köprü bağlantısını kaldırır.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


[Shape](../../com.aspose.cells/shape) nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Şekil çapa yer tutucusunun türünü ayarlar.

Bakınız [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir.

**Remarks**

Yalnızca resimler ve Ole Nesneleri için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Otomatik şekil türünü ayarlar.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Şeklin alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Bu şekil için oluşturma kimliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Nesnenin dekoratif olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Dolgu biçiminin görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Şeklin yatay olarak çevrilip çevrilmediğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Şeklin dikey olarak çevrilip çevrilmediğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Şeklin yazı tipini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Şeklin yüksekliğini santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Şeklin, üst ana şeklin kenarından dikey ofsetini, ana şeklin yüksekliğinin 1/4000 birimi olarak temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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


Bu metin kutusunda veri ve bazı biçimleri içeren HTML dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Denetimi doldurmak için kullanılan aralığı ayarlar.

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Denetimi doldurmak için kullanılan aralık. |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Şeklin üst şeklin sol kenarından yatay kaymasını, üst şeklin genişliğinin 1/4000'i biriminde temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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


Şeklin çalışma sayfası sol kenarından yatay ofsetini ayarlar.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Denetimin değerine bağlı aralığı ayarlar.

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Denetimin değerine bağlı aralık. |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


Doğru, şeklin en-boy oranının kilitlendiği anlamına gelir.

**Remarks**

Yalnızca resimler ve Ole Nesneleri için. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.IsAspectRatioLocked özelliğini kullanın. Bu özellik Temmuz 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya çalışma sayfasındaki nesneler korunduğunda anlamlı olduğunu unutmayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Kilitli özelliği ayarla.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Kilitli tür. |
| değer | boolean | Özelliğin değeri. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Şeklin sağ alt köşe sütunundan yatay ofsetini ayarlar.

**Remarks**

Değer aralığı 0 ile 1024 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Şeklin sağ alt köşe satırından dikey ofsetini ayarlar.

**Remarks**

Değer aralığı 0 ile 256 arasındadır.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Makronun adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Şeklin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Nesnenin yazdırılabilir olup olmadığını gösterir. False ise, bu şekil yazdırma sırasında basılmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Kenarlara uygulanacak bulanıklık yarıçapını, nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Bu şeklin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Bu nesne için metin akış yönünü ayarlar.

Bakınız [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Şeklin metin yatay hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Metin içeren şeklin metin yatay taşma türünü ayarlar.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Şeklin metin seçeneklerini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Şeklin metin yönlendirme türünü ayarlar.

Bakınız [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Önceden ayarlanmış metin şekli türünü ayarlar.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Şeklin metin dikey hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Metin içeren şeklin metin dikey taşma türünü ayarlar.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Şeklin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000'i biriminde dikey ofsetini temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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


Şeklin çalışma sayfası üst kenarından dikey kaydırmasını, piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Şeklin üst sol köşe sütunundan yatay kaydırmasını ayarlar.

**Remarks**

Değer aralığı 0 ile 1024 arasındadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Şeklin üst sol köşe satırından dikey kaydırmasını ayarlar.

**Remarks**

Değer aralığı 0 ile 256 arasındadır.

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


Üst satır indeksini temsil eder.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Şeklin genişliğini, üst şeklin 1/4000'i biriminde temsil eder.

**Remarks**

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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


Şeklin çalışma sayfası sol kenarından yatay kaydırmasını, piksel biriminde ayarlar.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Şekli öne getirir veya arkaya gönderir.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| orders | int | Sıfırdan küçükse, şekli arkaya ayarlar. Sıfırdan büyükse, şekli öne getirir. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Şekil görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.

**Remarks**

Aşağıdaki formatlar desteklenir: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Çıktı akışı. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Görüntünün kaydedileceği format. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Şekli bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Şekli bir dosyaya kaydeder.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Seçili değeri, bağlı hücrenin değeriyle günceller.

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

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

