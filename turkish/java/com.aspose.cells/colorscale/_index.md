---
title: "ColorScale"
second_title: "Aspose.Cells for Java API Referansı"
description: "ColorScale koşullu biçimlendirme kuralını açıklar."
type: docs
url: /tr/java/com.aspose.cells/colorscale/
---

**Inheritance:**
java.lang.Object
```
public class ColorScale
```

ColorScale koşullu biçimlendirme kuralını tanımlayın. Bu koşullu biçimlendirme kuralı hücrelerde kademeli bir renk ölçeği oluşturur.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getIs3ColorScale()](#getIs3ColorScale--) | Koşullu biçimlendirmenin 3 renk ölçeği olup olmadığını gösterir. |
| [getMaxCfvo()](#getMaxCfvo--) | Bu ColorScale'ın maksimum değer nesnesini alır. |
| [getMaxColor()](#getMaxColor--) | Aralıktaki maksimum değer için geçiş rengini alır. |
| [getMidCfvo()](#getMidCfvo--) | Bu ColorScale'ın orta değer nesnesini alır. |
| [getMidColor()](#getMidColor--) | Aralıktaki orta değer için geçiş rengini alır. |
| [getMinCfvo()](#getMinCfvo--) | Bu ColorScale'ın minimum değer nesnesini alır. |
| [getMinColor()](#getMinColor--) | Aralıktaki minimum değer için geçiş rengini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIs3ColorScale(boolean value)](#setIs3ColorScale-boolean-) | Koşullu biçimlendirmenin 3 renk ölçeği olup olmadığını gösterir. |
| [setMaxColor(Color value)](#setMaxColor-com.aspose.cells.Color-) | Aralıktaki maksimum değer için geçiş rengini ayarlar. |
| [setMidColor(Color value)](#setMidColor-com.aspose.cells.Color-) | Aralıktaki orta değer için geçiş rengini ayarlar. |
| [setMinColor(Color value)](#setMinColor-com.aspose.cells.Color-) | Aralıktaki minimum değer için geçiş rengini ayarlar. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIs3ColorScale() {#getIs3ColorScale--}
```
public boolean getIs3ColorScale()
```


Koşullu biçimlendirmenin 3 renk ölçeği olup olmadığını gösterir.

**Returns:**
boolean
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Bu ColorScale'ın maksimum değer nesnesini alır. Null veya FormatConditionValueType.Min tipinde CFValueObject ataması yapılamaz.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxColor() {#getMaxColor--}
```
public Color getMaxColor()
```


Aralıktaki maksimum değer için geçiş rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMidCfvo() {#getMidCfvo--}
```
public ConditionalFormattingValue getMidCfvo()
```


Bu ColorScale'ın orta değer nesnesini alır. FormatConditionValueType.Max veya FormatConditionValueType.Min tipinde CFValueObject ataması yapılamaz.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMidColor() {#getMidColor--}
```
public Color getMidColor()
```


Aralıktaki orta değer için geçiş rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Bu ColorScale'ın minimum değer nesnesini alır. Null veya FormatConditionValueType.Max tipinde CFValueObject ataması yapılamaz.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinColor() {#getMinColor--}
```
public Color getMinColor()
```


Aralıktaki minimum değer için geçiş rengini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
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




### setIs3ColorScale(boolean value) {#setIs3ColorScale-boolean-}
```
public void setIs3ColorScale(boolean value)
```


Koşullu biçimlendirmenin 3 renk ölçeği olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxColor(Color value) {#setMaxColor-com.aspose.cells.Color-}
```
public void setMaxColor(Color value)
```


Aralıktaki maksimum değer için geçiş rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMidColor(Color value) {#setMidColor-com.aspose.cells.Color-}
```
public void setMidColor(Color value)
```


Aralıktaki orta değer için geçiş rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setMinColor(Color value) {#setMinColor-com.aspose.cells.Color-}
```
public void setMinColor(Color value)
```


Aralıktaki minimum değer için geçiş rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

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

