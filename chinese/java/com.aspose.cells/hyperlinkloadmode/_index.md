---
title: "HyperlinkLoadMode"
second_title: "Aspose.Cells for Java API 参考"
description: "指定加载 HTML 时超链接的处理方式。"
type: docs
url: /zh/java/com.aspose.cells/hyperlinkloadmode/
---

**Inheritance:**
java.lang.Object
```
public final class HyperlinkLoadMode
```

指定加载 HTML 时超链接的处理方式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALLOW_MULTIPLE](#ALLOW-MULTIPLE) | 单元格中的所有超链接都会添加到 [Worksheet.getHyperlinks()](../../com.aspose.cells/worksheet\#getHyperlinks--)。 |
| [NORMAL](#NORMAL) | 仅加载单元格中的第一个超链接，后续的将被忽略。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALLOW_MULTIPLE {#ALLOW-MULTIPLE}
```
public static final int ALLOW_MULTIPLE
```


单元格中的所有超链接都会添加到 [Worksheet.getHyperlinks()](../../com.aspose.cells/worksheet\#getHyperlinks--)。请注意，MS Excel 本身仅支持每个单元格一个超链接，因此此选项可能生成 Excel 无法完全呈现的文件。

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


仅加载单元格中的第一个超链接，后续的将被忽略。

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

