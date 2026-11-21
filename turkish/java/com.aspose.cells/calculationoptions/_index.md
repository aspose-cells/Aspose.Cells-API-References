---
title: "CalculationOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hesaplama seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Hesaplama seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Formül hesaplamasının ilerlemesini izlemek için kullanıcı monitörü. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Formüller hesaplanırken karakterlerin kodlanması/çözülmesi için kullanılan kodlamayı belirtir. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru. |
| [getIgnoreError()](#getIgnoreError--) | Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Hesaplama hassasiyetinin işlenme stratejisini belirtir. |
| [getRecursive()](#getRecursive--) | Bir hücre hesaplanırken ve diğer hücrelere bağımlı olduğunda bağımlı hücrelerin özyinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Kullanıcının belirtilen formüller hesaplanmadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Formül hesaplamasının ilerlemesini izlemek için kullanıcı monitörü. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Formüller hesaplanırken karakterlerin kodlanması/çözülmesi için kullanılan kodlamayı belirtir. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Hesaplama hassasiyetinin işlenme stratejisini belirtir. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Bir hücre hesaplanırken ve diğer hücrelere bağımlı olduğunda bağımlı hücrelerin özyinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200'dür.

**Remarks**

Bağımlılık ağacında özyinelemeli olarak hesaplanması gereken çok sayıda hücre olduğunda, hesaplama sürecinde StackOverflowException oluşabilir. Bu durumda, kullanıcı bu özellik için daha küçük bir değer belirtmelidir. Böyle bir durumda, kullanıcı bu özelliğin uygun değerini gerçek formüller ve verilere göre belirlemelidir. Ancak çok küçük bir değer, formül hesaplamasının performansını düşürebilir ve 2'den küçük bir değer, başka birine bağımlı formülün hesaplanmasını imkansız kılar. Bu nedenle belirtilen değer 2'den küçükse, 2 olarak sıfırlanacaktır.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Formül hesaplamasının ilerlemesini izlemek için kullanıcı monitörü.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Formüller hesaplanırken karakterlerin kodlanması/kod çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç, bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek üzere uygun kodlamayı belirtebilir.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir. Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir. Varsayılan değer true'tır.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir.

**Remarks**

Örneğin [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) gibi, burada formüllerde kullanılan dış bağlantılar için veri kaynaklarını, özellikle INDIRECT işlevinde kullanılanları, belirtebilirsiniz. INDIRECT işlevinde kullanılan bu dış bağlantılar, çalışma kitabının dış bağlantılarının bir parçası olarak kabul edilmez ve [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) ile güncellenemez. Bu çalışma kitaplarının dış bağlantılarla eşleşmesi, [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) ve [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) tarafından belirlenir. Bu nedenle, her çalışma kitabı için [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) uygun bir değerle (genellikle ilgili [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) ile aynı olmalıdır) belirtilmiş olduğundan emin olun, böylece beklenen şekilde bağlanabilirler.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Hesaplama hassasiyetinin işlenme stratejisini belirtir.

Bakınız [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Bir hücre hesaplanırken ve diğer hücrelere bağımlı olduğunda bağımlı hücrelerin özyinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'tır.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir.

**Remarks**

Bu özellik açıkça belirtilmişse, belirtilen değer dinamik dizi formüllerinin yenilenip yenilenmeyeceğini belirlemek için kullanılır. Aksi takdirde ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) false ise), varsayılan değer, hangi tür formüllerin hesaplanacağına bağlıdır: Çalışma kitabı için formüller hesaplanırken, örneğin [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-) gibi, bu özellik true kabul edilir. Diğer durumlarda, örneğin [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) veya [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-) gibi, bu özellik false olarak alınır.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Kullanıcının belirtilen formüller hesaplanmadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200'dür.

**Remarks**

Bağımlılık ağacında özyinelemeli olarak hesaplanması gereken çok sayıda hücre olduğunda, hesaplama sürecinde StackOverflowException oluşabilir. Bu durumda, kullanıcı bu özellik için daha küçük bir değer belirtmelidir. Böyle bir durumda, kullanıcı bu özelliğin uygun değerini gerçek formüller ve verilere göre belirlemelidir. Ancak çok küçük bir değer, formül hesaplamasının performansını düşürebilir ve 2'den küçük bir değer, başka birine bağımlı formülün hesaplanmasını imkansız kılar. Bu nedenle belirtilen değer 2'den küçükse, 2 olarak sıfırlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Formül hesaplamasının ilerlemesini izlemek için kullanıcı monitörü.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Formüller hesaplanırken karakterlerin kodlanması/kod çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç, bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek üzere uygun kodlamayı belirtebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir. Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir. Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir.

**Remarks**

Örneğin [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) gibi, burada formüllerde kullanılan dış bağlantılar için veri kaynaklarını, özellikle INDIRECT işlevinde kullanılanları, belirtebilirsiniz. INDIRECT işlevinde kullanılan bu dış bağlantılar, çalışma kitabının dış bağlantılarının bir parçası olarak kabul edilmez ve [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) ile güncellenemez. Bu çalışma kitaplarının dış bağlantılarla eşleşmesi, [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) ve [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) tarafından belirlenir. Bu nedenle, her çalışma kitabı için [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) uygun bir değerle (genellikle ilgili [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) ile aynı olmalıdır) belirtilmiş olduğundan emin olun, böylece beklenen şekilde bağlanabilirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Hesaplama hassasiyetinin işlenme stratejisini belirtir.

Bakınız [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Bir hücre hesaplanırken ve diğer hücrelere bağımlı olduğunda bağımlı hücrelerin özyinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir.

**Remarks**

Bu özellik açıkça belirtilmişse, belirtilen değer dinamik dizi formüllerinin yenilenip yenilenmeyeceğini belirlemek için kullanılır. Aksi takdirde ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) false ise), varsayılan değer, hangi tür formüllerin hesaplanacağına bağlıdır: Çalışma kitabı için formüller hesaplanırken, örneğin [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-) gibi, bu özellik true kabul edilir. Diğer durumlarda, örneğin [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) veya [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-) gibi, bu özellik false olarak alınır.

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

