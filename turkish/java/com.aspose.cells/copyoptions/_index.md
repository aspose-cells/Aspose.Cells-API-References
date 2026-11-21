---
title: "CopyOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kopyalama seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Kopyalama seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Karakter biriminde sütun genişliğinin kopyalanıp kopyalanmayacağını gösterir. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Formül dest hedefi için geçerli değilse, yalnızca değerleri kopyalar. |
| [getCopyNames()](#getCopyNames--) | İsimlerin kopyalanıp kopyalanmayacağını gösterir. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Aralık, bitişik aralığa kopyalanırken genişletilip genişletilmeyeceğini gösterir. |
| [getKeepMacros()](#getKeepMacros--) | Makroların tutulup tutulmayacağını gösterir; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | Aynı dosyada aralığı kopyalarken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Başvurulan çalışma sayfası kopyalanmadıysa hedef çalışma sayfasına başvurulup başvurulmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Karakter biriminde sütun genişliğinin kopyalanıp kopyalanmayacağını gösterir. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Formül dest hedefi için geçerli değilse, yalnızca değerleri kopyalar. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | İsimlerin kopyalanıp kopyalanmayacağını gösterir. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Aralık, bitişik aralığa kopyalanırken genişletilip genişletilmeyeceğini gösterir. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Makroların tutulup tutulmayacağını gösterir; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | Aynı dosyada aralığı kopyalarken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Başvurulan çalışma sayfası kopyalanmadıysa hedef çalışma sayfasına başvurulup başvurulmayacağını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions yapıcı.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Karakter biriminde sütun genişliğinin kopyalanıp kopyalanmayacağını gösterir.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Formül dest hedefi için geçerli değilse, yalnızca değerleri kopyalar.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


İsimlerin kopyalanıp kopyalanmayacağını gösterir.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Aralık, bitişik aralığa kopyalanırken genişletilip genişletilmeyeceğini gösterir.

**Remarks**

Doğru ise, komşu satırlara bağlantılar kopyalanırken yeni bir bağlantı eklenmeden yalnızca bağlantının aralığı genişletilir.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Makroların tutulup tutulmayacağını gösterir;

**Remarks**

Yalnızca çalışma kitabı kopyalamak için.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


Aynı dosyada aralığı kopyalarken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. True ise kopyalanan grafiğin veri kaynağının hedef sayfaya başvuracağı anlamına gelir.

**Remarks**

Varsayılan değer false'tur, MS Excel gibi çalışır. Örneğin: veri kaynağı "sheet1!A1:B10" olan bir grafik, "sheet1" çalışma sayfasından "sheet2" başka bir çalışma sayfasına kopyalanırsa, veri kaynağı "sheet2!A1:B10" olarak değişir.

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabındaki aynı ada sahip çalışma sayfalarına başvurmasını isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır.

**Remarks**

Varsayılan değer true'tır.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Başvurulan çalışma sayfası kopyalanmadıysa hedef çalışma sayfasına başvurulup başvurulmayacağını gösterir.

**Remarks**

Yalnızca başka bir çalışma kitabından aralık veya çalışma sayfası kopyalanırken çalışır.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Karakter biriminde sütun genişliğinin kopyalanıp kopyalanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Formül dest hedefi için geçerli değilse, yalnızca değerleri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


İsimlerin kopyalanıp kopyalanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Aralık, bitişik aralığa kopyalanırken genişletilip genişletilmeyeceğini gösterir.

**Remarks**

Doğru ise, komşu satırlara bağlantılar kopyalanırken yeni bir bağlantı eklenmeden yalnızca bağlantının aralığı genişletilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Makroların tutulup tutulmayacağını gösterir;

**Remarks**

Yalnızca çalışma kitabı kopyalamak için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


Aynı dosyada aralığı kopyalarken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. True ise kopyalanan grafiğin veri kaynağının hedef sayfaya başvuracağı anlamına gelir.

**Remarks**

Varsayılan değer false'tur, MS Excel gibi çalışır. Örneğin: veri kaynağı "sheet1!A1:B10" olan bir grafik, "sheet1" çalışma sayfasından "sheet2" başka bir çalışma sayfasına kopyalanırsa, veri kaynağı "sheet2!A1:B10" olarak değişir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabındaki aynı ada sahip çalışma sayfalarına başvurmasını isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır.

**Remarks**

Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Başvurulan çalışma sayfası kopyalanmadıysa hedef çalışma sayfasına başvurulup başvurulmayacağını gösterir.

**Remarks**

Yalnızca başka bir çalışma kitabından aralık veya çalışma sayfası kopyalanırken çalışır.

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

