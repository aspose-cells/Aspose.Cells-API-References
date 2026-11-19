---
title: "超链接"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示超链接的对象。"
type: docs
url: /zh/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

封装表示超链接的对象。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [delete()](#delete--) | 删除此超链接 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | 表示超链接的地址。 |
| [getArea()](#getArea--) | 获取超链接的范围。 |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | 获取链接类型。 |
| [getScreenTip()](#getScreenTip--) | 返回或设置指定超链接的屏幕提示文本。 |
| [getTextToDisplay()](#getTextToDisplay--) | 表示指定超链接要显示的文本。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | 表示超链接的地址。 |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | 返回或设置指定超链接的屏幕提示文本。 |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | 表示指定超链接要显示的文本。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


删除此超链接

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddress() {#getAddress--}
```
public String getAddress()
```


表示超链接的地址。

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


获取超链接的范围。

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


获取链接类型。

参见 [TargetModeType](../../com.aspose.cells/targetmodetype)。

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


返回或设置指定超链接的屏幕提示文本。

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


表示指定超链接要显示的文本。默认值是超链接的地址。

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


表示超链接的地址。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


返回或设置指定超链接的屏幕提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


表示指定超链接要显示的文本。默认值是超链接的地址。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

