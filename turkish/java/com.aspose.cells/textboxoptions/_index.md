---
title: "TextBoxOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Şeklin metin seçeneklerini temsil eder"
type: docs
url: /tr/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Şeklin metin seçeneklerini temsil eder

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
         Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
         shape.setText("This is test.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Metnin şeklin dışına taşmasına izin verilip verilmeyeceği. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Alt kenar boşluğunu puan biriminde döndürür. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Sol kenar boşluğunu Nokta biriminde alır. |
| [getResizeToFitText()](#getResizeToFitText--) | Şekli metne sığdırmak için yeniden boyutlandırılıp boyutlandırılmayacağını gösterir |
| [getRightMarginPt()](#getRightMarginPt--) | Sağ kenar boşluğunu Nokta biriminde alır. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Belirli bir metin gövdesi içinde metin görüntüleme yönünü alır. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Excel'de "Format Shape - Text Options - Text Box - Vertical Alignment" ile eşleşir. |
| [getTopMarginPt()](#getTopMarginPt--) | Üst kenar boşluğunu Nokta biriminde alır. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Şekil içinde metin kaydırmayı belirtir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Metnin şeklin dışına taşmasına izin verilip verilmeyeceği. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Alt kenar boşluğunu puan biriminde döndürür. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Sol kenar boşluğunu Nokta biriminde ayarlar. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Şekli metne sığdırmak için yeniden boyutlandırılıp boyutlandırılmayacağını gösterir |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Sağ kenar boşluğunu Nokta biriminde ayarlar. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Belirli bir metin gövdesi içinde metin görüntüleme yönünü ayarlar. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Excel'de "Format Shape - Text Options - Text Box - Vertical Alignment" ile eşleşir. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Üst kenar boşluğunu Nokta biriminde ayarlar. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Şekil içinde metin kaydırmayı belirtir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Metnin şeklin dışına taşmasına izin verilip verilmeyeceği.

**Example**

```
         shape.getTextBoxOptions().setAllowTextToOverflow(true);
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
         shape.getTextBoxOptions().setBottomMarginPt(0.2d);
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


Sol kenar boşluğunu Nokta biriminde alır.

**Example**

```
         shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```

**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```


Şekli metne sığdırmak için yeniden boyutlandırılıp boyutlandırılmayacağını gösterir

**Example**

```
         shape.getTextBoxOptions().setResizeToFitText(true);
```

**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Sağ kenar boşluğunu Nokta biriminde alır.

**Example**

```
         shape.getTextBoxOptions().setRightMarginPt(0.2d);
```

**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```


Belirli bir metin gövdesi içinde metin görüntüleme yönünü alır. Excel'de "Format Shape - Text Options - Text Box - Text direction" ile eşdeğerdir.

Bak [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```

**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```


Excel'de "Format Shape - Text Options - Text Box - Vertical Alignment" ile eşleşir.

Bak [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Üst kenar boşluğunu Nokta biriminde alır.

**Example**

```
         shape.getTextBoxOptions().setTopMarginPt(0.2d);
```

**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```


Şekil içinde metin kaydırmayı belirtir. False - Metin gövdesinde kaydırma gerçekleşmez. True - Metin gövdesinde kaydırma gerçekleşir.

**Example**

```
         shape.getTextBoxOptions().setWrapTextInShape(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```


Metnin şeklin dışına taşmasına izin verilip verilmeyeceği.

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


Sol kenar boşluğunu Nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Şekli metne sığdırmak için yeniden boyutlandırılıp boyutlandırılmayacağını gösterir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Sağ kenar boşluğunu Nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Belirli bir metin gövdesi içinde metin görüntüleme yönünü ayarlar. Excel'de "Format Shape - Text Options - Text Box - Text direction" ile eşdeğerdir.

Bak [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Excel'de "Format Shape - Text Options - Text Box - Vertical Alignment" ile eşleşir.

Bak [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Üst kenar boşluğunu Nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Şekil içinde metin kaydırmayı belirtir. False - Metin gövdesinde kaydırma gerçekleşmez. True - Metin gövdesinde kaydırma gerçekleşir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

