---
title: "QueryTable"
second_title: "Aspose.Cells for Java API Referansı"
description: "QueryTable bilgisini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/querytable/
---

**Inheritance:**
java.lang.Object
```
public class QueryTable
```

QueryTable bilgisini temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Getting the first query table in the worksheet if exists
         //QueryTable qt = worksheet.QueryTables[0];
         //Getting display address of the query table.
         //string address = qt.ResultRange.Address;
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar. |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | Sorgu tablosunun bağlantı kimliğini alır. |
| [getExternalConnection()](#getExternalConnection--) | İlgili dış bağlantıyı alır. |
| [getName()](#getName--) | Sorgu tablosunun adını alır. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar. |
| [getResultRange()](#getResultRange--) | Sonucun aralığını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar. |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```


Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Sorgu tablosunun bağlantı kimliğini alır.

**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```


İlgili dış bağlantıyı alır.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```


Sorgu tablosunun adını alır.

**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar.

**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```


Sonucun aralığını alır.

**Returns:**
[Range](../../com.aspose.cells/range) - 
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




### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```


Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar.

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

