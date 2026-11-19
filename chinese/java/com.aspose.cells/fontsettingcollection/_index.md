---
title: "FontSettingCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示列表。"
type: docs
url: /zh/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

表示 [FontSetting](../../com.aspose.cells/fontsetting) 的列表。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [appendText(String text)](#appendText-java.lang.String-) | 追加文本。 |
| [clear()](#clear--) | 清除所有设置。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [deleteText(int index, int count)](#deleteText-int-int-) | 删除一些字符。 |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | 使用字体设置格式化文本。 |
| [get(int index)](#get-int-) | 通过索引获取 [FontSetting](../../com.aspose.cells/fontsetting)。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getHtmlString()](#getHtmlString--) | 获取此形状中包含数据和一些格式的 html 字符串。 |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | 获取段落的枚举器。 |
| [getText()](#getText--) | 获取形状的文本。 |
| [getTextAlignment()](#getTextAlignment--) | 表示文本主体的对齐设置。 |
| [getTextParagraphs()](#getTextParagraphs--) | 获取所有段落。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | 在该位置插入索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | 替换文本。 |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 替换文本。 |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | 设置此形状中包含数据和一些格式的 html 字符串。 |
| [setText(String value)](#setText-java.lang.String-) | 设置形状的文本。 |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | 设置预设的 WordArt 样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


追加文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 文本。 |

### clear() {#clear--}
```
public void clear()
```


清除所有设置。

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


删除一些字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 起始索引。 |
| 计数 | int | 字符的计数。 |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


使用字体设置格式化文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |
| length | int | 长度。 |
| font | [Font](../../com.aspose.cells/font) | 字体。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 字体的标志。 |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


通过索引获取 [FontSetting](../../com.aspose.cells/fontsetting)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


获取此形状中包含数据和一些格式的 html 字符串。

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


获取段落的枚举器。

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


获取形状的文本。

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


表示文本主体的对齐设置。

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


获取所有段落。

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


在该位置插入索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 起始索引。 |
| 文本 | java.lang.String | 文本。 |

### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的项的零基索引。 |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


替换文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 起始索引。 |
| 计数 | int | 字符的计数。 |
| 文本 | java.lang.String | 文本。 |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


替换文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | java.lang.String | 旧文本。 |
| newValue | java.lang.String | 新文本。 |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


设置此形状中包含数据和一些格式的 html 字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置形状的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


设置预设的 WordArt 样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). 预设的 WordArt 样式. |

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

