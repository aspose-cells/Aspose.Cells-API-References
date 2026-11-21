---
title: "Koruma"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfası için mevcut çeşitli koruma seçenekleri tiplerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Bir çalışma sayfası için mevcut çeşitli koruma seçenekleri tiplerini temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Koruma bilgilerini kopyala. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Korunan bir çalışma sayfasında sütun silmenin izin verilip verilmediğini temsil eder. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Korunan bir çalışma sayfasında satır silmenin izin verilip verilmediğini temsil eder. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder. |
| [getAllowFiltering()](#getAllowFiltering--) | Koruma uygulanmadan önce oluşturulan bir AutoFilter'ı kullanma izni olup olmadığını temsil eder. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Korunan bir çalışma sayfasında hücre biçimlendirmesine izin verilip verilmediğini temsil eder. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Korunan bir çalışma sayfasında sütun biçimlendirmesine izin verilip verilmediğini temsil eder |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Korunan bir çalışma sayfasında satır biçimlendirmesine izin verilip verilmediğini temsil eder |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Korunan bir çalışma sayfasında kullanıcının kilitli hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Korunan bir çalışma sayfasında kullanıcının kilidi açılmış hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [getAllowSorting()](#getAllowSorting--) | Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Korunan bir çalışma sayfasında kullanıcının özet tabloyu (pivot table) manipüle etmesine izin verilip verilmediğini temsil eder. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Çalışma sayfasını korumak için kullanılan şifreyi temsil eder. |
| [getPasswordHash()](#getPasswordHash--) | Mevcut şifrenin karmasını alır. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Çalışma sayfasının şifreyle korunup korunmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Korunan bir çalışma sayfasında sütun silmenin izin verilip verilmediğini temsil eder. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Korunan bir çalışma sayfasında satır silmenin izin verilip verilmediğini temsil eder. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Koruma uygulanmadan önce oluşturulan bir AutoFilter'ı kullanma izni olup olmadığını temsil eder. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Korunan bir çalışma sayfasında hücre biçimlendirmesine izin verilip verilmediğini temsil eder. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Korunan bir çalışma sayfasında sütun biçimlendirmesine izin verilip verilmediğini temsil eder |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Korunan bir çalışma sayfasında satır biçimlendirmesine izin verilip verilmediğini temsil eder |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Korunan bir çalışma sayfasında kullanıcının kilitli hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Korunan bir çalışma sayfasında kullanıcının kilidi açılmış hücreleri seçmesine izin verilip verilmediğini temsil eder. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Korunan bir çalışma sayfasında kullanıcının özet tabloyu (pivot table) manipüle etmesine izin verilip verilmediğini temsil eder. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Çalışma sayfasını korumak için kullanılan şifreyi temsil eder. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Şifreyi doğrular. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Koruma bilgilerini kopyala.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Korunan bir çalışma sayfasında sütun silmenin izin verilip verilmediğini temsil eder.

**Remarks**

Silinecek hücreleri içeren sütunlar, sayfa korunduğunda kilidi açılmış olmalı ve "Kilitli olmayan hücreleri seç" seçeneği etkinleştirilmiş olmalıdır.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Korunan bir çalışma sayfasında satır silmenin izin verilip verilmediğini temsil eder.

**Remarks**

Silinecek hücreleri içeren satırlar, sayfa korunduğunda kilidi açılmış olmalı ve "Kilitli olmayan hücreleri seç" seçeneği etkinleştirilmiş olmalıdır.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Koruma uygulanmadan önce oluşturulan bir AutoFilter'ı kullanma izni olup olmadığını temsil eder.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Korunan bir çalışma sayfasında hücre biçimlendirmesine izin verilip verilmediğini temsil eder.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Korunan bir çalışma sayfasında sütun biçimlendirmesine izin verilip verilmediğini temsil eder

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Korunan bir çalışma sayfasında satır biçimlendirmesine izin verilip verilmediğini temsil eder

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Korunan bir çalışma sayfasında kullanıcının kilitli hücreleri seçmesine izin verilip verilmediğini temsil eder.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Korunan bir çalışma sayfasında kullanıcının kilidi açılmış hücreleri seçmesine izin verilip verilmediğini temsil eder.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Korunan bir çalışma sayfasında kullanıcının özet tabloyu (pivot table) manipüle etmesine izin verilip verilmediğini temsil eder.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Çalışma sayfasını korumak için kullanılan şifreyi temsil eder.

**Remarks**

Şifre null veya boş bir dize olarak ayarlanırsa, çalışma sayfasını veya çalışma kitabını şifre kullanmadan korumasını kaldırabilirsiniz. Aksi takdirde, çalışma sayfasının veya çalışma kitabının korumasını kaldırmak için şifre belirtmeniz gerekir.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Mevcut şifrenin karmasını alır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Çalışma sayfasının şifreyle korunup korunmadığını gösterir.

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




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


Korunan bir çalışma sayfasında sütun silmenin izin verilip verilmediğini temsil eder.

**Remarks**

Silinecek hücreleri içeren sütunlar, sayfa korunduğunda kilidi açılmış olmalı ve "Kilitli olmayan hücreleri seç" seçeneği etkinleştirilmiş olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Korunan bir çalışma sayfasında satır silmenin izin verilip verilmediğini temsil eder.

**Remarks**

Silinecek hücreleri içeren satırlar, sayfa korunduğunda kilidi açılmış olmalı ve "Kilitli olmayan hücreleri seç" seçeneği etkinleştirilmiş olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Korunan bir çalışma sayfasında kilitli hücrelerin içeriğini düzenleme izni olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Korunan bir çalışma sayfasında çizim nesnelerini manipüle etme izni olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Korunan bir çalışma sayfasında senaryoları düzenleme izni olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Koruma uygulanmadan önce oluşturulan bir AutoFilter'ı kullanma izni olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Korunan bir çalışma sayfasında hücre biçimlendirmesine izin verilip verilmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Korunan bir çalışma sayfasında sütun biçimlendirmesine izin verilip verilmediğini temsil eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Korunan bir çalışma sayfasında satır biçimlendirmesine izin verilip verilmediğini temsil eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Korunan bir çalışma sayfasında kullanıcının kilitli hücreleri seçmesine izin verilip verilmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Korunan bir çalışma sayfasında kullanıcının kilidi açılmış hücreleri seçmesine izin verilip verilmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Korunan bir çalışma sayfasında sıralama seçeneğinin izin verilip verilmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Korunan bir çalışma sayfasında kullanıcının özet tabloyu (pivot table) manipüle etmesine izin verilip verilmediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Çalışma sayfasını korumak için kullanılan şifreyi temsil eder.

**Remarks**

Şifre null veya boş bir dize olarak ayarlanırsa, çalışma sayfasını veya çalışma kitabını şifre kullanmadan korumasını kaldırabilirsiniz. Aksi takdirde, çalışma sayfasının veya çalışma kitabının korumasını kaldırmak için şifre belirtmeniz gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Şifreyi doğrular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Şifre. |

**Returns:**
boolean -
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

