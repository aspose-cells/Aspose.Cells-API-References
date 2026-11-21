---
title: "ExternalLink"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma kitabındaki harici bir bağlantıyı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Bir çalışma kitabındaki harici bir bağlantıyı temsil eder.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Harici bir ad ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Harici bağlantının veri kaynağını temsil eder. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Harici bağlantının depolanmış veri kaynağını temsil eder. |
| [getPathType()](#getPathType--) | Bu harici bağlantının yol türünü al. |
| [getType()](#getType--) | Harici bağlantının türünü alır. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Bu dış bağlantının diğerleri tarafından referans alınıp alınmadığını gösterir. |
| [isVisible()](#isVisible--) | Bu dış bağlantının MS Excel'de görünür olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Harici bağlantının veri kaynağını temsil eder. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Harici bağlantının depolanmış veri kaynağını temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Harici bir ad ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Dış adın metni. Dış ad bir çalışma sayfasına aitse, metin Sheet1!Text şeklinde olmalıdır. |
| referTo | java.lang.String | Dış adın referTo özelliği. Bir hücre veya aralık olmalıdır. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Harici bağlantının veri kaynağını temsil eder.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Harici bağlantının depolanmış veri kaynağını temsil eder.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Bu harici bağlantının yol türünü al.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Harici bağlantının türünü alır.

Bakınız [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Bu dış bağlantının diğerleri tarafından referans alınıp alınmadığını gösterir.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Bu dış bağlantının MS Excel'de görünür olup olmadığını gösterir.

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




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


Harici bağlantının veri kaynağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Harici bağlantının depolanmış veri kaynağını temsil eder.

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

