---
title: "FormulaSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Formüllerin ve hesaplamanın ayarları."
type: docs
url: /tr/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Formüllerin ve hesaplamanın ayarları.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [getCalculationId()](#getCalculationId--) | Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir. |
| [getCalculationMode()](#getCalculationMode--) | MS Excel'de çalışma kitabı hesaplama modunu alır. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Dairesel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir. |
| [getMaxChange()](#getMaxChange--) | Dairesel referansı çözmek için maksimum değişim. |
| [getMaxIteration()](#getMaxIteration--) | Dairesel referansı çözmek için maksimum yineleme sayısı. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | MS Excel'de çalışma kitabı hesaplama modunu ayarlar. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Dairesel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir. |
| [setMaxChange(double value)](#setMaxChange-double-) | Dairesel referansı çözmek için maksimum değişim. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Dairesel referansı çözmek için maksimum yineleme sayısı. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir.

**Remarks**

Bu özellik yalnızca ayarları ortaya çıkan elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken buna göre hareket edebilir. Çoğu kullanıcı uygulaması için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. ms excel durumunda, bu özelliğin değeri, sonucu açan uygulamayla ilişkili yeniden hesaplama motoru tanımlayıcısından daha düşükse, uygulama dosyayı yükledikten hemen sonra bu çalışma kitabındaki tüm formüllerin sonuçlarını yeniden hesaplar. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


MS Excel'de çalışma kitabı hesaplama modunu alır.

Bak [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Performans düşünülerek, çoğu kullanıcının uygulaması için, bu özellik için hangi mod ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz. Kullanıcı formülleri hesaplaması gerektiğinde, lütfen gereksinime göre farklı nesnelerdeki yöntemleri her zaman çağırın: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur.

**Remarks**

Çalışma kitabında çok sayıda formül olduğunda ve kullanıcı yalnızca küçük bir kısmını değiştirerek bunları tekrar tekrar hesaplaması gerektiğinde, performans açısından hesaplama zincirini etkinleştirmek yararlı olabilir. Öte yandan, zincir etkinleştirildiğinde, zincir modelinin korunması ekstra bellek gerektirir ve hücre değerini veya formülleri değiştirme gibi bazı diğer işlemler için biraz daha fazla CPU süresi gerekir. Bu özellik false'tan true'ya değiştirildikten sonra, hesaplama zinciri ilk hesaplama sırasında analiz edilir ve oluşturulur, bu yüzden ilk hesaplama için gereken süre zincirsiz normal hesaplamadan daha uzun olabilir.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Dairesel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Dairesel referansı çözmek için maksimum değişim.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Dairesel referansı çözmek için maksimum yineleme sayısı.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Formül tokenları arasında eklenen boşluk ve satır sonlarının, formüller alınırken ve ayarlanırken korunup korunmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Genellikle bu boşluk ve satır sonları sadece görsel amaçlıdır, korunup korunmamaları hesaplanan sonucu etkilemez. Performans düşünülerek, özel bir gereksinim yoksa, formüller işlenirken bunları korumamak daha iyidir.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir.

**Remarks**

Bu özellik yalnızca ayarları ortaya çıkan elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken buna göre hareket edebilir. Çoğu kullanıcı uygulaması için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. ms excel durumunda, bu özelliğin değeri, sonucu açan uygulamayla ilişkili yeniden hesaplama motoru tanımlayıcısından daha düşükse, uygulama dosyayı yükledikten hemen sonra bu çalışma kitabındaki tüm formüllerin sonuçlarını yeniden hesaplar. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


MS Excel'de çalışma kitabı hesaplama modunu ayarlar.

Bak [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Performans düşünülerek, çoğu kullanıcının uygulaması için, bu özellik için hangi mod ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz. Kullanıcı formülleri hesaplaması gerektiğinde, lütfen gereksinime göre farklı nesnelerdeki yöntemleri her zaman çağırın: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur.

**Remarks**

Çalışma kitabında çok sayıda formül olduğunda ve kullanıcı yalnızca küçük bir kısmını değiştirerek bunları tekrar tekrar hesaplaması gerektiğinde, performans açısından hesaplama zincirini etkinleştirmek yararlı olabilir. Öte yandan, zincir etkinleştirildiğinde, zincir modelinin korunması ekstra bellek gerektirir ve hücre değerini veya formülleri değiştirme gibi bazı diğer işlemler için biraz daha fazla CPU süresi gerekir. Bu özellik false'tan true'ya değiştirildikten sonra, hesaplama zinciri ilk hesaplama sırasında analiz edilir ve oluşturulur, bu yüzden ilk hesaplama için gereken süre zincirsiz normal hesaplamadan daha uzun olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Dairesel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken buna göre davranabilir. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özellik için hangi değer ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


Dairesel referansı çözmek için maksimum değişim.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Dairesel referansı çözmek için maksimum yineleme sayısı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Formül tokenları arasında eklenen boşluk ve satır sonlarının, formüller alınırken ve ayarlanırken korunup korunmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Genellikle bu boşluk ve satır sonları sadece görsel amaçlıdır, korunup korunmamaları hesaplanan sonucu etkilemez. Performans düşünülerek, özel bir gereksinim yoksa, formüller işlenirken bunları korumamak daha iyidir.

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

