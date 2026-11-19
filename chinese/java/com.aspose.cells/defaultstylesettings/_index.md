---
title: "DefaultStyleSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "工作簿样式属性默认值的设置。"
type: docs
url: /zh/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

工作簿样式属性默认值的设置。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | 指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。 |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | 获取工作簿的默认字体名称 |
| [getFontSize()](#getFontSize--) | 获取工作簿的默认标准字体大小。 |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | 获取水平对齐的默认值 |
| [getVerticalAlignment()](#getVerticalAlignment--) | 获取垂直对齐的默认值 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | 指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。 |
| [setFontName(String value)](#setFontName-java.lang.String-) | 设置工作簿的默认字体名称 |
| [setFontSize(double value)](#setFontSize-double-) | 设置工作簿的默认标准字体大小。 |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | 设置水平对齐的默认值 |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | 设置垂直对齐的默认值 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。默认值为 false，这意味着默认情况下，只要某个样式的自定义模式不为空，就会使用自定义模式来格式化值。

**Remarks**

从现有模板文件加载工作簿时，可能会为同一样式同时定义内置数字和自定义模式。此属性决定在使用该样式格式化值时，应使用内置数字还是自定义模式。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


获取工作簿的默认字体名称

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


获取工作簿的默认标准字体大小。

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


获取水平对齐的默认值

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


获取垂直对齐的默认值

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。默认值为 false，这意味着默认情况下，只要某个样式的自定义模式不为空，就会使用自定义模式来格式化值。

**Remarks**

从现有模板文件加载工作簿时，可能会为同一样式同时定义内置数字和自定义模式。此属性决定在使用该样式格式化值时，应使用内置数字还是自定义模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


设置工作簿的默认字体名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


设置工作簿的默认标准字体大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


设置水平对齐的默认值

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


设置垂直对齐的默认值

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

