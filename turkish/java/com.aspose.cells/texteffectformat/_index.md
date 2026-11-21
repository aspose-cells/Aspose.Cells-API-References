---
title: "TextEffectFormat"
second_title: "Aspose.Cells for Java API Referansı"
description: "WordArt nesnelerine uygulanan özellik ve yöntemleri içerir."
type: docs
url: /tr/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

WordArt nesnelerine uygulanan özellik ve yöntemleri içerir.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
         TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
         textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
         workbook.save("Book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Yazı tipinin kalın olup olmadığını gösterir. |
| [getFontItalic()](#getFontItalic--) | Yazı tipinin italik olup olmadığını gösterir. |
| [getFontName()](#getFontName--) | WordArt'ta kullanılan yazı tipinin adı. |
| [getFontSize()](#getFontSize--) | WordArt'ta kullanılan yazı tipinin boyutu (puan olarak). |
| [getPresetShape()](#getPresetShape--) | Önceden ayarlanmış şekil tipini alır. |
| [getRotatedChars()](#getRotatedChars--) | Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür. |
| [getText()](#getText--) | WordArt'taki metin. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Yazı tipinin kalın olup olmadığını gösterir. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Yazı tipinin italik olup olmadığını gösterir. |
| [setFontName(String value)](#setFontName-java.lang.String-) | WordArt'ta kullanılan yazı tipinin adı. |
| [setFontSize(int value)](#setFontSize-int-) | WordArt'ta kullanılan yazı tipinin boyutu (puan olarak). |
| [setPresetShape(int value)](#setPresetShape-int-) | Önceden ayarlanmış şekil tipini ayarlar. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür. |
| [setText(String value)](#setText-java.lang.String-) | WordArt'taki metin. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Önceden ayarlanmış metin efektini ayarlar. |
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
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```


Yazı tipinin kalın olup olmadığını gösterir.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Yazı tipinin italik olup olmadığını gösterir.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


WordArt'ta kullanılan yazı tipinin adı.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


WordArt'ta kullanılan yazı tipinin boyutu (puan olarak).

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Önceden ayarlanmış şekil tipini alır.

Bak [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


WordArt'taki metin.

**Returns:**
java.lang.String
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




### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```


Yazı tipinin kalın olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Yazı tipinin italik olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


WordArt'ta kullanılan yazı tipinin adı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


WordArt'ta kullanılan yazı tipinin boyutu (puan olarak).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Önceden ayarlanmış şekil tipini ayarlar.

Bak [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


WordArt'taki metin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Önceden ayarlanmış metin efektini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Önceden ayarlanmış metin efekti. |

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

