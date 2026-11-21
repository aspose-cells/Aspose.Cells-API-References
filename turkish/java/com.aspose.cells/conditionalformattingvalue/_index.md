---
title: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir gradient ölçeği dataBar veya iconSet içindeki ara nokta değerlerini açıklar."
type: docs
url: /tr/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Bir renk geçiş ölçeği, veri çubuğu veya simge kümesindeki ara nokta değerlerini açıklar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Bu koşullu biçimlendirme değer nesnesinin tipini alır. |
| [getValue()](#getValue--) | Bu koşullu biçimlendirme değer nesnesinin değerini alır. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Büyük veya Eşit bayrağını alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Büyük veya Eşit bayrağını ayarlar. |
| [setType(int value)](#setType-int-) | Bu koşullu biçimlendirme değer nesnesinin tipini ayarlar. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Bu koşullu biçimlendirme değer nesnesinin değerini ayarlar. |
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
### getType() {#getType--}
```
public int getType()
```


Bu koşullu biçimlendirme değer nesnesinin tipini alır. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, \"Value\" değerini otomatik olarak null yapar.

[FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype) sayfasına bakın.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Bu koşullu biçimlendirme değer nesnesinin değerini alır. Tip ile birlikte kullanılmalıdır.

**Remarks**

Değer bir dize olup \"=\" ile başlıyorsa, formül olarak işlenir; aksi takdirde basit bir değer olarak işlenir.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Büyük veya Eşit bayrağını alır. Yalnızca ikon setleri için kullanılır, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmadığını belirler. 'false' değeri, 'büyük' operatörünün kullanıldığını gösterir. Varsayılan değer true'tır.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Büyük veya Eşit bayrağını ayarlar. Yalnızca ikon setleri için kullanılır, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmadığını belirler. 'false' değeri, 'büyük' operatörünün kullanılacağını gösterir. Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Bu koşullu biçimlendirme değer nesnesinin tipini ayarlar. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, \"Value\" değerini otomatik olarak null yapar.

[FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype) sayfasına bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Bu koşullu biçimlendirme değer nesnesinin değerini ayarlar. Tip ile birlikte kullanılmalıdır.

**Remarks**

Değer bir dize olup \"=\" ile başlıyorsa, formül olarak işlenir; aksi takdirde basit bir değer olarak işlenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

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

