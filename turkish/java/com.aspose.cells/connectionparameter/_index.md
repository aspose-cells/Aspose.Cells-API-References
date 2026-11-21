---
title: "ConnectionParameter"
second_title: "Aspose.Cells for Java API Referansı"
description: "Harici veri bağlantılarıyla kullanılan parametrelerle ilgili özellikleri belirtir. Parametreler ODBC ve web sorguları için geçerlidir."
type: docs
url: /tr/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Harici veri bağlantılarıyla kullanılan parametrelerle ilgili özellikleri belirtir. Parametreler ODBC ve web sorguları için geçerlidir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Sorgu parametresi için kullanılacak hücrenin değerini gösteren hücre referansı. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Parametrenin adı. |
| [getPrompt()](#getPrompt--) | Parametre için istem dizesi. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Parametre değerini sağlayan hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren işaret. |
| [getSqlType()](#getSqlType--) | Parametrenin SQL veri tipi. |
| [getType()](#getType--) | Kullanılan parametre türü. |
| [getValue()](#getValue--) | Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, metin değeri veya Boolean değeri. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Sorgu parametresi için kullanılacak hücrenin değerini gösteren hücre referansı. |
| [setName(String value)](#setName-java.lang.String-) | Parametrenin adı. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Parametre için istem dizesi. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Parametre değerini sağlayan hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren işaret. |
| [setSqlType(int value)](#setSqlType-int-) | Parametrenin SQL veri tipi. |
| [setType(int value)](#setType-int-) | Kullanılan parametre türü. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, metin değeri veya Boolean değeri. |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Sorgu parametresi için kullanılacak hücrenin değerini gösteren hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır.

**Returns:**
java.lang.String
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


Parametrenin adı.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Parametre için istem dizesi. Harici veriler yenilenmeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Parametre değerini sağlayan hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren işaret. Doğru ise, her değişiklikte yeni parametre değeri kullanılarak harici veri yenilenir. Yanlış ise, harici veri yalnızca kullanıcı tarafından talep edildiğinde veya başka bir olay (ör. çalışma kitabı açıldığında) yenilemeyi tetiklediğinde yenilenir.

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir.

Bakınız [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca \{boolean, double, integer, or string\} öğelerinden birinin belirtilmesi beklenir.

Bakınız [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, metin değeri veya Boolean değeri. Yalnızca parameterType değer olduğunda kullanılır.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Sorgu parametresi için kullanılacak hücrenin değerini gösteren hücre referansı. Yalnızca parameterType hücre olduğunda kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Parametrenin adı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Parametre için istem dizesi. Harici veriler yenilenmeden önce parametre değerini toplamak için giriş UI'siyle birlikte elektronik tablo kullanıcısına sunulur. Yalnızca parameterType = prompt olduğunda kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Parametre değerini sağlayan hücrenin içeriği değiştiğinde sorgunun otomatik olarak yenilenip yenilenmeyeceğini gösteren işaret. Doğru ise, her değişiklikte yeni parametre değeri kullanılarak harici veri yenilenir. Yanlış ise, harici veri yalnızca kullanıcı tarafından talep edildiğinde veya başka bir olay (ör. çalışma kitabı açıldığında) yenilemeyi tetiklediğinde yenilenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


Parametrenin SQL veri tipi. Yalnızca ODBC kaynakları için geçerlidir.

Bakınız [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Kullanılan parametre türü. parameterType=value ise, boolean, double, integer veya string değerlerinden biri kullanılacaktır. Bu durumda, yalnızca \{boolean, double, integer, or string\} öğelerinden birinin belirtilmesi beklenir.

Bakınız [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Sorgu parametresi olarak kullanılacak tam sayı olmayan sayısal değer, tam sayı değeri, metin değeri veya Boolean değeri. Yalnızca parameterType değer olduğunda kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

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

