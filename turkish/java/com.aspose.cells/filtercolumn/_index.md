---
title: "FilterColumn"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tek bir sütun veya tabloda bir sütun için filtreyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Tek bir sütun veya tabloda bir sütun için filtreyi temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Renk ile veri filtrelemek için [ColorFilter](../../com.aspose.cells/colorfilter) alır. |
| [getCustomFilters()](#getCustomFilters--) | Özel ölçütlerle veri filtrelemek için [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) alır. |
| [getDynamicFilter()](#getDynamicFilter--) | Dinamik ölçütlerle filtrelemek için [getDynamicFilter()](../../com.aspose.cells/filtercolumn\\#getDynamicFilter--) alır. |
| [getFieldIndex()](#getFieldIndex--) | Aralıktaki sütun ofsetini alır. |
| [getFilter()](#getFilter--) | Filtreleme verisinin koşulunu alır. |
| [getFilterType()](#getFilterType--) | Filtreleme verisinin tipini alır. |
| [getFilterValues()](#getFilterValues--) | Etiketler veya tarih saat ile veri filtrelemek için [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) alır. |
| [getIconFilter()](#getIconFilter--) | Simgeye göre veri filtrelemek için [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) alır. |
| [getMultipleFilters()](#getMultipleFilters--) | Etiketler veya tarih saat ile veri filtrelemek için [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) alır. |
| [getTop10Filter()](#getTop10Filter--) | Veri sıralamasına göre veri filtrelemek için [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) alır. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Tümünü seçer. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Özel ölçütlerle veri filtrelemek için [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) alır. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Aralıktaki sütun ofsetini ayarlar. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Filtreleme verisinin koşulunu ayarlar. |
| [setFilterType(int value)](#setFilterType-int-) | Filtreleme verisinin tipini ayarlar. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Etiketler veya tarih saat ile veri filtrelemek için [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) alır. |
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
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


Renk ile veri filtrelemek için [ColorFilter](../../com.aspose.cells/colorfilter) alır.

**Remarks**

İlk olarak [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--)'i [FilterType.COLOR_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) olarak ayarlar, aksi takdirde Null döndürülür.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Özel ölçütlerle veri filtrelemek için [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) alır.

**Remarks**

NOT: Bu özelliğin ayarlayıcısı artık kullanımdan kaldırılmıştır. Bunun yerine, [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) özelliğini [FilterType.CUSTOM_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS) olarak ayarlayın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Dinamik ölçütlerle filtrelemek için [getDynamicFilter()](../../com.aspose.cells/filtercolumn\\#getDynamicFilter--) alır.

**Remarks**

Bu özelliği kullanmadan önce, lütfen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--)'in [FilterType.DYNAMIC_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER) olduğundan emin olun, aksi takdirde null döndürülür.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Aralıktaki sütun ofsetini alır.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Filtreleme verisinin koşulunu alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--)'e göre ilgili özelliği kullanın. Ayrıca, [FilterType.MULTIPLE_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) filtre tipi için döndürülen nesne artık [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) yerine [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)'dır. Bu özellik, Ekim 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Filtreleme verisinin tipini alır.

Bakınız [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Bu özellik ayarlandığında ilgili filtre nesnesi oluşturulur ve ilgili özellik, filtre nesnesini almak için kullanılmalıdır:

| FilterType | Özellik |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


Etiketler veya tarih saat ile veri filtrelemek için [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) alır.

**Remarks**

İlk olarak [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) işlevini [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) olarak ayarlar, aksi takdirde Null döndürülecektir.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Simgeye göre veri filtrelemek için [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) alır.

**Remarks**

Bu özelliği kullanmadan önce, lütfen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) işlevinin [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER) olduğundan emin olun, aksi takdirde null döndürülecektir.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Etiketler veya tarih saat ile veri filtrelemek için [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen FilterColumn.FilterValues özelliğini kullanın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Veri sıralamasına göre veri filtrelemek için [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) alır.

**Remarks**

Bu özelliği kullanmadan önce, lütfen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) işlevinin [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10) olduğundan emin olun, aksi takdirde null döndürülecektir.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


Tümünü seçer.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Özel ölçütlerle veri filtrelemek için [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) alır.

**Remarks**

NOT: Bu özelliğin ayarlayıcısı artık kullanımdan kaldırılmıştır. Bunun yerine, [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) özelliğini [FilterType.CUSTOM_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS) olarak ayarlayın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Aralıktaki sütun ofsetini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Filtreleme verisinin koşulunu ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--)'e göre ilgili özelliği kullanın. Ayrıca, [FilterType.MULTIPLE_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) filtre tipi için döndürülen nesne artık [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) yerine [FilterValueCollection](../../com.aspose.cells/filtervaluecollection)'dır. Bu özellik, Ekim 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Filtreleme verisinin tipini ayarlar.

Bakınız [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Bu özellik ayarlandığında ilgili filtre nesnesi oluşturulur ve ilgili özellik, filtre nesnesini almak için kullanılmalıdır:

| FilterType | Özellik |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Etiketler veya tarih saat ile veri filtrelemek için [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen FilterColumn.FilterValues özelliğini kullanın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

