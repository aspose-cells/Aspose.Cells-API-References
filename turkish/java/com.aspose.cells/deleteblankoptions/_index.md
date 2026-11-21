---
title: "DeleteBlankOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Boş hücreleri/satırları/sütunları silme ayarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Boş hücreleri/satırları/sütunları silme ayarını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini belirtir. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Bir hücrenin formül olduğu ve hesaplanan sonucun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini belirtir. |
| [getEndIndex()](#getEndIndex--) | Boş satır/sütunları kontrol edip silmek için aralığın son satır/sütun indeksini (dahil) belirtir. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Silme nedeniyle oluşan değişiklikleri izlemek için monitörü alır. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Boş satır/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini belirtir. |
| [getStartIndex()](#getStartIndex--) | Boş satır/sütunu kontrol edip silmek için aralığın başlangıç satır/sütun indeksini belirtir. |
| [getUpdateReference()](#getUpdateReference--) | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini belirtir. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Bir hücrenin formül olduğu ve hesaplanan sonucun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini belirtir. |
| [setEndIndex(int value)](#setEndIndex-int-) | Boş satır/sütunları kontrol edip silmek için aralığın son satır/sütun indeksini (dahil) belirtir. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Silme nedeniyle oluşan değişiklikleri izlemek için monitörü ayarlar. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Boş satır/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini belirtir. |
| [setStartIndex(int value)](#setStartIndex-int-) | Boş satır/sütunu kontrol edip silmek için aralığın başlangıç satır/sütun indeksini belirtir. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Bu özellik false olarak ayarlandığında, çizim nesneleri tarafından kapsanan tüm satır/sütunlar boş olarak kabul edilmez ve silinmez.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Bir hücrenin formül olduğu ve hesaplanan sonucunun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. Varsayılan değer false'tur.

**Remarks**

Genellikle kullanıcı, bu özellik true iken silme işlemi yapılmadan önce formüllerin hesaplandığından emin olmalıdır. Aksi takdirde, [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) gibi normal API'ler tarafından yeni oluşturulan tüm formüller boş olarak kabul edilir ve hesaplamadan önce sonuçları null olduğu için silinebilir.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Kontrol edilecek ve boş satır/sütunların silineceği aralığın son satır/sütun indeksini (dahil) belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Silme nedeniyle oluşan değişiklikleri izlemek için monitörü alır.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Boş satır/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini belirtir.

Bakınız [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

[MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) için, içindeki tüm hücreler boş olmayan sol üst hücre dışındaki hücreler boş olarak kabul edilir. Bu, bu özelliğin varsayılan değeridir.

[MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) için, içindeki tüm hücreler boş olmayan olarak kabul edilir.

[MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) için, içerik görüntüleme alanının dışındaki tüm hücreler boş olarak kabul edilir.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Boş satır/sütunu kontrol edip silmek için aralığın başlangıç satır/sütun indeksini belirtir.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir.

**Remarks**

26.7 sürümünden itibaren bu özelliğin varsayılan değeri true olarak ayarlandı.

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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Bu özellik false olarak ayarlandığında, çizim nesneleri tarafından kapsanan tüm satır/sütunlar boş olarak kabul edilmez ve silinmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Bir hücrenin formül olduğu ve hesaplanan sonucunun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. Varsayılan değer false'tur.

**Remarks**

Genellikle kullanıcı, bu özellik true iken silme işlemi yapılmadan önce formüllerin hesaplandığından emin olmalıdır. Aksi takdirde, [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) gibi normal API'ler tarafından yeni oluşturulan tüm formüller boş olarak kabul edilir ve hesaplamadan önce sonuçları null olduğu için silinebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Kontrol edilecek ve boş satır/sütunların silineceği aralığın son satır/sütun indeksini (dahil) belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Silme nedeniyle oluşan değişiklikleri izlemek için monitörü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Boş satır/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini belirtir.

Bakınız [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

[MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) için, içindeki tüm hücreler boş olmayan sol üst hücre dışındaki hücreler boş olarak kabul edilir. Bu, bu özelliğin varsayılan değeridir.

[MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) için, içindeki tüm hücreler boş olmayan olarak kabul edilir.

[MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) için, içerik görüntüleme alanının dışındaki tüm hücreler boş olarak kabul edilir.



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Boş satır/sütunu kontrol edip silmek için aralığın başlangıç satır/sütun indeksini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir.

**Remarks**

26.7 sürümünden itibaren bu özelliğin varsayılan değeri true olarak ayarlandı.

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

