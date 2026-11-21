---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma kitabının ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Çalışma kitabının ayarlarını temsil eder.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Dosyanın yazarını alır. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini belirtir, varsayılan false dır. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Hesaplanan formüller zincirinin oluşturulup oluşturulmayacağını belirtir. |
| [getDate1904()](#getDate1904--) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır. |
| [getEnableMacros()](#getEnableMacros--) | Makroları etkinleştir; Şu anda yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplanıp hesaplanmayacağını belirtir. |
| [getIteration()](#getIteration--) | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını belirtir. |
| [getMaxIteration()](#getMaxIteration--) | Dairesel bir referansı çözmek için maksimum yineleme sayısını döndürür veya ayarlar, varsayılan değer 100'dür. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Dosyanın yazarını ayarlar. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini belirtir, varsayılan false dır. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Hesaplanan formüller zincirinin oluşturulup oluşturulmayacağını belirtir. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri ayarlar. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Makroları etkinleştir; Şu anda yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplanıp hesaplanmayacağını belirtir. |
| [setIteration(boolean value)](#setIteration-boolean-) | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını belirtir. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Dairesel bir referansı çözmek için maksimum yineleme sayısını döndürür veya ayarlar, varsayılan değer 100'dür. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini belirtir, varsayılan false dır.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Excel dosyasının kısıtlamalarının, kullanıcı hücre ilgili nesneleri değiştirdiğinde kontrol edilip edilmediğini belirtir. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik true ise bir Exception alırsınız. Bu özellik false ise girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. varsayılan değer false'tur.

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


Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Makroları etkinleştir; Şu anda yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplanıp hesaplanmayacağını belirtir.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını belirtir.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Dairesel bir referansı çözmek için maksimum yineleme sayısını döndürür veya ayarlar, varsayılan değer 100'dür.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Bu çalışma kitabındaki hesaplamalar yalnızca sayılar ekranda gösterildiği hassasiyetle yapılacaksa doğru.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'dur.

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


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini belirtir, varsayılan false dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Excel dosyasının kısıtlamalarının, kullanıcı hücre ilgili nesneleri değiştirdiğinde kontrol edilip edilmediğini belirtir. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik true ise bir Exception alırsınız. Bu özellik false ise girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Makroları etkinleştir; Şu anda yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplanıp hesaplanmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Dairesel bir referansı çözmek için maksimum yineleme sayısını döndürür veya ayarlar, varsayılan değer 100'dür.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'dur.

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

