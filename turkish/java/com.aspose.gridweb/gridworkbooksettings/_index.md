---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma kitabının ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Çalışma kitabının ayarlarını temsil eder.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | varsayılan yapıcı |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Dosyanın yazarını alır. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini alır. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Hesaplanan formüller zincirinin oluşturulup oluşturulmadığını alır. |
| [getDate1904()](#getDate1904--) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden değeri alır. |
| [getEnableMacros()](#getEnableMacros--) | Makroların etkinleştirilip etkinleştirilmediğini alır; Şu anda yalnızca bir çalışma kitabındaki bir sayfayı başka bir sayfaya kopyalarken çalışır. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplayıp hesaplamadığını alır. |
| [getIteration()](#getIteration--) | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmadığını alır. |
| [getMaxIteration()](#getMaxIteration--) | Döngüsel bir referansı çözmek için azami yineleme sayısını alır, varsayılan değer 100'dür. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmadığını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Dosyanın yazarını ayarlar. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini ayarlar. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını ayarlar. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden değeri ayarlar. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Makroların etkinleştirilip etkinleştirilmeyeceğini ayarlar; artık yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplayıp hesaplamayacağını ayarlar. |
| [setIteration(boolean value)](#setIteration-boolean-) | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını ayarlar. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Döngüsel bir referansı çözmek için azami yineleme sayısını ayarlar, varsayılan değer 100'dür. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


varsayılan yapıcı

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Dosyanın yazarını alır.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini alır.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Hesaplanmış formül zincirinin oluşturulup oluşturulmadığını alır. Varsayılan değeri false'tur.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden değeri alır.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Makroların etkinleştirilip etkinleştirilmediğini alır; Şu anda yalnızca bir çalışma kitabındaki bir sayfayı başka bir sayfaya kopyalarken çalışır.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplayıp hesaplamadığını alır.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Döngüsel referansları çözmek için yineleme kullanılıp kullanılmadığını alır.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Döngüsel bir referansı çözmek için azami yineleme sayısını alır, varsayılan değer 100'dür.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Genellikle bu boşluk ve satır sonları sadece görsel amaçlıdır, korunup korunmamaları hesaplanan sonucu etkilemez. Performans düşünülerek, özel bir gereksinim yoksa, formüller işlenirken bunları korumamak daha iyidir.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmadığını alır.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Dosyanın yazarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını ayarlar. Varsayılan değeri false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Makroların etkinleştirilip etkinleştirilmeyeceğini ayarlar; artık yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplayıp hesaplamayacağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Döngüsel bir referansı çözmek için azami yineleme sayısını ayarlar, varsayılan değer 100'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Genellikle bu boşluk ve satır sonları sadece görsel amaçlıdır, korunup korunmamaları hesaplanan sonucu etkilemez. Performans düşünülerek, özel bir gereksinim yoksa, formüller işlenirken bunları korumamak daha iyidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını ayarlar.

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

