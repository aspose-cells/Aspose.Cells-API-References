---
title: "ProtectedRange"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sayfa koruması AÇIK olduğunda düzenlemeye izin verilen belirtilen aralık."
type: docs
url: /tr/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Sayfa koruması AÇIK olduğunda düzenlemeye izin verilen belirtilen aralık.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Bu nesneye bir başvurulan alan ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Tüm başvurulan alanları alır. |
| [getCellArea()](#getCellArea--) | Alır [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) nesnesi, korunacak hücre alanını temsil eder. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Aralık başlığını alır. |
| [getPassword()](#getPassword--) | Aralığı korumak için kullanılan şifreyi temsil eder. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre sağlamadan bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Çalışma sayfasının şifreyle korunup korunmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Aralık başlığını alır. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Aralığı korumak için kullanılan şifreyi temsil eder. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre sağlamadan bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Bu nesneye bir başvurulan alan ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu. |
| endRow | int | Bitiş satırı. |
| endColumn | int | Bitiş sütunu. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Tüm başvurulan alanları alır.

**Returns:**
com.aspose.cells.CellArea[] - Tüm başvurulan alanları döndürür.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Alır [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) nesnesi, korunacak hücre alanını temsil eder.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Aralık başlığını alır. Bu, adlandırılmış bir aralık tanımı yerine bir tanımlayıcı olarak kullanılır.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Aralığı korumak için kullanılan şifreyi temsil eder.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre sağlamadan bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar.

**Returns:**
java.lang.String
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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Aralık başlığını alır. Bu, adlandırılmış bir aralık tanımı yerine bir tanımlayıcı olarak kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Aralığı korumak için kullanılan şifreyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre sağlamadan bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar.

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

