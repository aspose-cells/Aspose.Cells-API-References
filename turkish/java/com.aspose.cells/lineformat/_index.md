---
title: "LineFormat"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çizginin tüm ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Çizginin tüm ayarlarını temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin, belirtilen başka bir [LineFormat](../../com.aspose.cells/lineformat) nesnesiyle aynı değere sahip olup olmadığını belirler. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Çizginin başlangıç ok uzunluğu tipini alır. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Çizginin başlangıç ok tipini alır. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Çizginin başlangıç ok genişliği tipini alır. |
| [getCapType()](#getCapType--) | Bitiş kapaklarını belirtir. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Çizgi birleşik tipini belirtir. |
| [getDashStyle()](#getDashStyle--) | Çizgi kesikli tipini belirtir. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Çizginin bitiş ok uzunluğu tipini alır. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Çizginin bitiş ok tipini alır. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Çizginin bitiş ok genişliği tipini alır. |
| [getFillType()](#getFillType--) | Dolgu tipini alır |
| [getGradientColor1()](#getGradientColor1--) | Belirtilen dolgu için geçiş rengi 1'i döndürür. |
| [getGradientColor2()](#getGradientColor2--) | Belirtilen dolgu için geçiş rengi 2'yi döndürür. |
| [getGradientColorType()](#getGradientColorType--) | Belirtilen dolgu için geçiş renk tipini döndürür. |
| [getGradientDegree()](#getGradientDegree--) | Belirtilen dolgu için geçiş derecesini döndürür. |
| [getGradientFill()](#getGradientFill--) | Alır [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) nesnesini. |
| [getGradientStyle()](#getGradientStyle--) | Belirtilen dolgu için geçiş stilini döndürür. |
| [getGradientVariant()](#getGradientVariant--) | Belirtilen dolgu için geçiş varyantını döndürür. |
| [getImageData()](#getImageData--) | Resim veri bilgisini alır. |
| [getJoinType()](#getJoinType--) | Çizgi birleşim tipini belirtir. |
| [getPattern()](#getPattern--) | Bir alanın görüntü desenini temsil eder. |
| [getPatternFill()](#getPatternFill--) | Alır [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) nesnesini. |
| [getPictureFormatType()](#getPictureFormatType--) | Resim formatı tipini alır. |
| [getPresetColor()](#getPresetColor--) | Belirtilen dolgu için geçiş ön ayar rengini döndürür. |
| [getScale()](#getScale--) | Resim formatı ölçeğini alır. |
| [getSetType()](#getSetType--) | Dolgu formatı ayar tipini alır. |
| [getSolidFill()](#getSolidFill--) | Alır [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) nesnesini. |
| [getTexture()](#getTexture--) | Belirtilen dolgu için doku tipini temsil eder. |
| [getTextureFill()](#getTextureFill--) | Alır [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) nesnesini. |
| [getTransparency()](#getTransparency--) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [getType()](#getType--) | Dolgu tipini alır. |
| [getWeight()](#getWeight--) | Çizginin ağırlığını puan biriminde alır. |
| [hashCode()](#hashCode--) | Karma kodunu alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Çizginin başlangıç ok uzunluğu tipini ayarlar. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Çizginin başlangıç ok tipini ayarlar. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Çizginin başlangıç ok genişliği tipini ayarlar. |
| [setCapType(int value)](#setCapType-int-) | Bitiş kapaklarını belirtir. |
| [setCompoundType(int value)](#setCompoundType-int-) | Çizgi birleşik tipini belirtir. |
| [setDashStyle(int value)](#setDashStyle-int-) | Çizgi kesikli tipini belirtir. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Satırın son ok uzunluğu türünü ayarlar. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Satırın son ok tipini ayarlar. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Satırın son ok genişliği türünü ayarlar. |
| [setFillType(int value)](#setFillType-int-) | Dolgu tipini ayarlar |
| [setImageData(byte[] value)](#setImageData-byte---) | Resim veri bilgisini ayarlar. |
| [setJoinType(int value)](#setJoinType-int-) | Çizgi birleşim tipini belirtir. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. |
| [setPattern(int value)](#setPattern-int-) | Bir alanın görüntü desenini temsil eder. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Resim formatı türünü ayarlar. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Belirtilen dolguyu ön ayarlı renk geçişine ayarlar. |
| [setScale(double value)](#setScale-double-) | Resim formatı ölçeğini ayarlar. |
| [setSetType(int value)](#setSetType-int-) | Dolgu formatı ayar tipini alır. |
| [setTexture(int value)](#setTexture-int-) | Belirtilen dolgu için doku tipini temsil eder. |
| [setTransparency(double value)](#setTransparency-double-) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setType(int value)](#setType-int-) | Doldurma tipini ayarlar. |
| [setWeight(double value)](#setWeight-double-) | Satırın ağırlığını nokta biriminde ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin, belirtilen başka bir [LineFormat](../../com.aspose.cells/lineformat) nesnesiyle aynı değere sahip olup olmadığını belirler.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         LineFormat obj = workbook.getWorksheets().get(0).getShapes().get(0).getLine();
         if (lineFmt.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak [LineFormat](../../com.aspose.cells/lineformat) nesnesi. |

**Returns:**
boolean - obj parametresinin değeri bu örneğin değeriyle aynıysa true; aksi takdirde false. obj null ise, bu yöntem false döndürür.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Çizginin başlangıç ok uzunluğu tipini alır.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```


Çizginin başlangıç ok tipini alır.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```


Çizginin başlangıç ok genişliği tipini alır.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setBeginArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Bitiş kapaklarını belirtir.

Bakınız [LineCapType](../../com.aspose.cells/linecaptype).

**Example**

```
         lineFmt.setCapType(LineCapType.FLAT);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Çizgi birleşik tipini belirtir.

Bakınız [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Example**

```
         lineFmt.setCompoundType(MsoLineStyle.SINGLE);
```

**Returns:**
int
### getDashStyle() {#getDashStyle--}
```
public int getDashStyle()
```


Çizgi kesikli tipini belirtir.

Bakınız [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Example**

```
         lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```

**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```


Çizginin bitiş ok uzunluğu tipini alır.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```


Çizginin bitiş ok tipini alır.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```


Çizginin bitiş ok genişliği tipini alır.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Dolgu tipini alır

Bakın [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Belirtilen dolgu için geçiş rengi 1'i döndürür.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Belirtilen dolgu için geçiş rengi 2'yi döndürür.

**Remarks**

Yalnızca degrade renk tipi GradientColorType.TwoColors olduğunda, bu özellik anlamlıdır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Belirtilen dolgu için geçiş renk tipini döndürür.

Bakın [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Belirtilen doldurma için degrade derecesini döndürür. Yalnızca Excel 2007 için geçerlidir.

**Remarks**

Yalnızca 0.0 (koyu) ile 1.0 (açık) arasında bir değer olabilir.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Alır [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) nesnesini.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Belirtilen dolgu için geçiş stilini döndürür.

Bak [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Belirtilen doldurma için degrade varyantını döndürür. Yalnızca Excel 2007 için geçerlidir.

**Remarks**

Yalnızca 1 ile 4 arasında bir değer olabilir; bu değer, Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Resim veri bilgisini alır.

**Remarks**

Doldurma biçimi özel doku biçimi değilse, null döndürür.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Çizgi birleşim tipini belirtir.

Bakınız [LineJoinType](../../com.aspose.cells/linejointype).

**Example**

```
         lineFmt.setJoinType(LineJoinType.ROUND);
```

**Returns:**
int
### getPattern() {#getPattern--}
```
public int getPattern()
```


Bir alanın görüntü desenini temsil eder.

[FillPattern](../../com.aspose.cells/fillpattern) öğesine bakın.

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Alır [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) nesnesini.

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Resim formatı tipini alır.

Bak [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Belirtilen dolgu için geçiş ön ayar rengini döndürür.

Bakın [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Resim formatı ölçeğini alır.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Dolgu formatı ayar tipini alır.

Bakın [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Alır [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) nesnesini.

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Belirtilen dolgu için doku tipini temsil eder.

Bakınız [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Alır [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) nesnesini.

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Dolgu tipini alır.

Bakın [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Çizginin ağırlığını puan biriminde alır.

**Example**

```
         lineFmt.setWeight(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Karma kodunu alır.

**Example**

```
         int hashCode = lineFmt.hashCode();
```

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBeginArrowheadLength(int value) {#setBeginArrowheadLength-int-}
```
public void setBeginArrowheadLength(int value)
```


Çizginin başlangıç ok uzunluğu tipini ayarlar.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Çizginin başlangıç ok tipini ayarlar.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Çizginin başlangıç ok genişliği tipini ayarlar.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Bitiş kapaklarını belirtir.

Bakınız [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Çizgi birleşik tipini belirtir.

Bakınız [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Çizgi kesikli tipini belirtir.

Bakınız [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Satırın son ok uzunluğu türünü ayarlar.

Bakınız [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Satırın son ok tipini ayarlar.

Bakınız [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Satırın son ok genişliği türünü ayarlar.

Bakınız [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Dolgu tipini ayarlar

Bakın [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Resim veri bilgisini ayarlar.

**Remarks**

Doldurma biçimi özel doku biçimi değilse, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Çizgi birleşim tipini belirtir.

Bakınız [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Belirtilen doldurmayı tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| derece | double | Degrade derecesi. 0.0 (karanlık) ile 1.0 (açık) arasında bir değer olabilir. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Bir alanın görüntü desenini temsil eder.

[FillPattern](../../com.aspose.cells/fillpattern) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Resim formatı türünü ayarlar.

Bak [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Belirtilen doldurmayı önceden tanımlı renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Önceden tanımlı renk tipi |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Resim formatı ölçeğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Dolgu formatı ayar tipini alır.

Bakın [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Belirtilen dolgu için doku tipini temsil eder.

Bakınız [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| transparency1 | double | color1'in şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| transparency2 | double | color2'nin şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Doldurma tipini ayarlar.

Bakın [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Satırın ağırlığını nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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

