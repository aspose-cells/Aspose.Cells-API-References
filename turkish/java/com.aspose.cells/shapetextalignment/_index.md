---
title: "ShapeTextAlignment"
second_title: "Aspose.Cells for Java API Referansı"
description: "Şekillerin metin hizalama ayarını temsil eder"
type: docs
url: /tr/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

şeklin metin hizalama ayarını temsil eder;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin, belirtilen başka bir [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) nesnesiyle aynı değere sahip olup olmadığını belirler. |
| [getAutoSize()](#getAutoSize--) | Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Alt kenar boşluğunu puan biriminde döndürür. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Sol kenar boşluğunu puan biriminde döndürür. |
| [getNumberOfColumns()](#getNumberOfColumns--) | Sınırlayıcı dikdörtgendeki metin sütun sayısını alır. |
| [getRightMarginPt()](#getRightMarginPt--) | Sağ kenar boşluğunu puan biriminde döndürür. |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Şekil ile metnin döndürülüp döndürülmediğini gösterir. |
| [getRotationAngle()](#getRotationAngle--) | Şeklin dönüşünü alır. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Metin kutusunun yatay taşma tipini alır. |
| [getTextShapeType()](#getTextShapeType--) | Metnin dönüşüm tipini alır. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Metin kutusunun dikey taşma tipini alır. |
| [getTextVerticalType()](#getTextVerticalType--) | Metin yönünü alır. |
| [getTopMarginPt()](#getTopMarginPt--) | Üst kenar boşluğunu puan biriminde döndürür. |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir. |
| [isLockedText()](#isLockedText--) | Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir. |
| [isTextWrapped()](#isTextWrapped--) | Metin içeren şeklin metin kaydırma türünü alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Alt kenar boşluğunu puan biriminde döndürür. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Sol kenar boşluğunu puan biriminde döndürür. |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Sınırlayıcı dikdörtgendeki metin sütun sayısını ayarlar. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Sağ kenar boşluğunu puan biriminde döndürür. |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Şekil ile metnin döndürülüp döndürülmediğini gösterir. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Şeklin dönüşünü ayarlar. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Metin kutusunun yatay taşma tipini ayarlar. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Metnin dönüşüm tipini ayarlar. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Metin kutusunun dikey taşma tipini ayarlar. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Metin yönünü ayarlar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Metin içeren şeklin metin sarma türünü ayarlar. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Üst kenar boşluğunu puan biriminde döndürür. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin, belirtilen başka bir [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) nesnesiyle aynı değere sahip olup olmadığını belirler.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnekle karşılaştırmak için [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) nesnesi. |

**Returns:**
boolean - obj parametresinin değeri bu örneğin değeriyle aynıysa true; aksi takdirde false. obj null ise, bu yöntem false döndürür.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir.

**Example**

```
         shapeTextAlignment.setAutoSize(false);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


Alt kenar boşluğunu puan biriminde döndürür.

**Example**

```
         shapeTextAlignment.setBottomMarginPt(2.0d);
```

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```


Sol kenar boşluğunu puan biriminde döndürür.

**Example**

```
         shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Sınırlayıcı dikdörtgendeki metin sütun sayısını alır.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Sağ kenar boşluğunu puan biriminde döndürür.

**Example**

```
         shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


Şekil ile metnin döndürülüp döndürülmediğini gösterir.

**Example**

```
         shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Şeklin dönüşünü alır.

**Example**

```
         shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Metin kutusunun yatay taşma tipini alır.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Metnin dönüşüm tipini alır.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         //Usually do not modify this value unless you know exactly what the modification will result in
         shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Metin kutusunun dikey taşma tipini alır.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


Metin yönünü alır.

Bak [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Üst kenar boşluğunu puan biriminde döndürür.

**Example**

```
         shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir.

**Example**

```
         shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```


Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir.

**Remarks**

Yalnızca çalışma sayfası korunduğunda çalışır.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Metin içeren şeklin metin kaydırma türünü alır.

**Example**

```
         shapeTextAlignment.setTextWrapped(true);
```

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




### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```


Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Alt kenar boşluğunu puan biriminde döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Sol kenar boşluğunu puan biriminde döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir.

**Remarks**

Yalnızca çalışma sayfası korunduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Sınırlayıcı dikdörtgendeki metin sütun sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Sağ kenar boşluğunu puan biriminde döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Şekil ile metnin döndürülüp döndürülmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Şeklin dönüşünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Metin kutusunun yatay taşma tipini ayarlar.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Metnin dönüşüm tipini ayarlar.

Bakınız [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Metin kutusunun dikey taşma tipini ayarlar.

Bakınız [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Metin yönünü ayarlar.

Bak [TextVerticalType](../../com.aspose.cells/textverticaltype).

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

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Üst kenar boşluğunu puan biriminde döndürür.

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

