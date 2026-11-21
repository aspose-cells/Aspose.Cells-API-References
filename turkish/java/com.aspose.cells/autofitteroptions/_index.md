---
title: "AutoFitterOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Temsil eder tüm otomatik sığdırıcı seçeneklerini."
type: docs
url: /tr/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Temsil eder tüm otomatik sığdırıcı seçeneklerini.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Satırda hücreler birleştirildiğinde satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Birleştirilmiş hücrelerin satır yüksekliğini otomatik ayarlama türünü alır. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Kaydırılmış metnin otomatik ayarlama türünü alır. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Varsayılan düzenleme dilini alır. |
| [getForRendering()](#getForRendering--) | Renderleme amacı için ayarlanıp ayarlanmayacağını gösterir. |
| [getFormatStrategy()](#getFormatStrategy--) | Biçimlendirilmiş stratejiyi alır. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Gizli satırları/sütunları yok sayar. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Satırları otomatik ayarlarken maksimum satır yüksekliğini (Point biriminde) alır. |
| [getOnlyAuto()](#getOnlyAuto--) | Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Satırda hücreler birleştirildiğinde satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma türünü ayarlar. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Satır içi kaydırılmış metnin otomatik sığdırma türünü ayarlar. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Varsayılan düzenleme dilini ayarlar. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Renderleme amacı için ayarlanıp ayarlanmayacağını gösterir. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Biçimlendirilmiş stratejiyi ayarlar. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Gizli satırları/sütunları yok sayar. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Satırları otomatik sığdırırken maksimum satır yüksekliğini (Point biriminde) ayarlar. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Hücreler bir satırda birleştirildiğinde satır yüksekliğinin otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen AutoFitterOptions.AutoFitMergedCellsType özelliğini kullanın. Bu özellik Aralık 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Birleştirilmiş hücrelerin satır yüksekliğini otomatik ayarlama türünü alır.

Bak [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel, satır yüksekliğini ayarlarken birleştirilmiş hücreleri varsayılan olarak yok sayar, bu nedenle Aspose.Cells de MS Excel varsayılanı gibi çalışır. Lütfen bu türü ayarlayarak birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma şeklini değiştirin.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Kaydırılmış metnin otomatik ayarlama türünü alır.

Bak [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Varsayılan düzenleme dilini alır.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Renderleme amacı için ayarlanıp ayarlanmayacağını gösterir.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Biçimlendirilmiş stratejiyi alır.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Performans için varsayılan değer CellStyle'dır.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Gizli satırları/sütunları yok sayar.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Satırları otomatik ayarlarken maksimum satır yüksekliğini (Point biriminde) alır.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Hücreler bir satırda birleştirildiğinde satır yüksekliğinin otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen AutoFitterOptions.AutoFitMergedCellsType özelliğini kullanın. Bu özellik Aralık 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma türünü ayarlar.

Bak [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel, satır yüksekliğini ayarlarken birleştirilmiş hücreleri varsayılan olarak yok sayar, bu nedenle Aspose.Cells de MS Excel varsayılanı gibi çalışır. Lütfen bu türü ayarlayarak birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma şeklini değiştirin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Satır içi kaydırılmış metnin otomatik sığdırma türünü ayarlar.

Bak [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Varsayılan düzenleme dilini ayarlar.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Renderleme amacı için ayarlanıp ayarlanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Biçimlendirilmiş stratejiyi ayarlar.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Performans için varsayılan değer CellStyle'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Gizli satırları/sütunları yok sayar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Satırları otomatik sığdırırken maksimum satır yüksekliğini (Point biriminde) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir.

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

