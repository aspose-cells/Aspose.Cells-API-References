---
title: "Köprü"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir köprüyi temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Bir köprüyi temsil eden nesneyi kapsüller.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [delete()](#delete--) | Bu bağlantıyı siler |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Bir bağlantının adresini temsil eder. |
| [getArea()](#getArea--) | Bağlantının aralığını alır. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Bağlantı türünü alır. |
| [getScreenTip()](#getScreenTip--) | Belirtilen bağlantı için ScreenTip metnini alır veya ayarlar. |
| [getTextToDisplay()](#getTextToDisplay--) | Belirtilen bağlantı için görüntülenecek metni temsil eder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Bir bağlantının adresini temsil eder. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Belirtilen bağlantı için ScreenTip metnini alır veya ayarlar. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Belirtilen bağlantı için görüntülenecek metni temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Bu bağlantıyı siler

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
### getAddress() {#getAddress--}
```
public String getAddress()
```


Bir bağlantının adresini temsil eder.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


Bağlantının aralığını alır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Bağlantı türünü alır.

Bakın [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Belirtilen bağlantı için ScreenTip metnini alır veya ayarlar.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Belirtilen bağlantı için görüntülenecek metni temsil eder. Varsayılan değer, bağlantının adresidir.

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Bir bağlantının adresini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Belirtilen bağlantı için ScreenTip metnini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Belirtilen bağlantı için görüntülenecek metni temsil eder. Varsayılan değer, bağlantının adresidir.

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

