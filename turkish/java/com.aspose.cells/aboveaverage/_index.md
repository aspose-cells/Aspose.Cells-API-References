---
title: "AboveAverage"
second_title: "Aspose.Cells for Java API Referansı"
description: "AboveAverage koşullu biçimlendirme kuralını açıklayın."
type: docs
url: /tr/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

AboveAverage koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki veya altındaki hücreleri vurgular.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | Koşullu biçimlendirme kuralında ortalamanın üzerindeki veya altındaki standart sapma sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | "Ortalamanın üzerindeki" kural olup olmadığını gösteren bayrağı alır. |
| [isEqualAverage()](#isEqualAverage--) | 'aboveAverage' ve 'belowAverage' kriterlerinin ortalamayı dahil edip etmediğini veya dışarıda bıraktığını gösteren bayrağı alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | "Ortalamanın üzerindeki" kural olup olmadığını gösteren bayrağı ayarlar. |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | Ortalamanın kendisini kapsayıp kapsamadığını veya o değerden dışarıda olup olmadığını gösteren 'aboveAverage' ve 'belowAverage' kriterleri için bayrağı ayarlar. |
| [setStdDev(int value)](#setStdDev-int-) | Koşullu biçimlendirme kuralında ortalamanın üstünde veya altında dahil edilecek standart sapma sayısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
```


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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


Koşullu biçimlendirme kuralında ortalamanın üstünde veya altında dahil edilecek standart sapma sayısını alır. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'dır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


"Ortalamanın üzeri" kuralı olup olmadığını gösteren bayrağı alır. 'true' 'ortalamanın üzeri' anlamına gelir. Varsayılan değer true'dur.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


'aboveAverage' ve 'belowAverage' kriterlerinin ortalamayı kapsayıp kapsamadığını gösteren bayrağı alır, ya da o değerden dışarıda olup olmadığını. 'true' ortalama değerinin kriterlere dahil edileceğini gösterir. Varsayılan değer false'tur.

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




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


"Ortalamanın üzeri" kuralı olup olmadığını gösteren bayrağı ayarlar. 'true' 'ortalamanın üzeri' anlamına gelir. Varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


'aboveAverage' ve 'belowAverage' kriterlerinin ortalamayı kapsayıp kapsamadığını gösteren bayrağı ayarlar, ya da o değerden dışarıda olup olmadığını. 'true' ortalama değerinin kriterlere dahil edileceğini gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


Koşullu biçimlendirme kuralında ortalamanın üstünde veya altında dahil edilecek standart sapma sayısını ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'dır.

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

