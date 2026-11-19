---
title: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "一组内置文档属性的集合。"
type: docs
url: /zh/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

一组内置文档属性的集合。

**Remarks**

提供通过名称（使用索引器）访问对象的方式，以及通过一组返回适当类型值的强类型属性。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [contains(String name)](#contains-java.lang.String-) | 如果集合中存在具有指定名称的属性，则返回 true。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。 |
| [get(String name)](#get-java.lang.String-) | 通过属性名称返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。 |
| [getAuthor()](#getAuthor--) | 获取文档作者的名称。 |
| [getBytes()](#getBytes--) | 表示文档中字节数的估计值。 |
| [getCategory()](#getCategory--) | 获取文档的类别。 |
| [getCharacters()](#getCharacters--) | 表示文档中字符数的估计值。 |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | 表示文档中字符数（包括空格）的估计值。 |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | 获取文档注释。 |
| [getCompany()](#getCompany--) | 获取公司属性。 |
| [getContentStatus()](#getContentStatus--) | 获取文档的内容状态。 |
| [getContentType()](#getContentType--) | 获取文档的内容类型。 |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getCreatedTime()](#getCreatedTime--) | 获取文档创建日期（本地时区）。 |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | 获取文档创建的通用时间。 |
| [getDocumentVersion()](#getDocumentVersion--) | 表示文件的版本。 |
| [getHyperlinkBase()](#getHyperlinkBase--) | 获取 hyperlinkbase 属性。 |
| [getKeywords()](#getKeywords--) | 获取文档关键字。 |
| [getLanguage()](#getLanguage--) | 获取文档语言。 |
| [getLastPrinted()](#getLastPrinted--) | 获取文档上次打印的日期（本地时区）。 |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | 获取文档上次打印的通用时间。 |
| [getLastSavedBy()](#getLastSavedBy--) | 获取最后作者的姓名。 |
| [getLastSavedTime()](#getLastSavedTime--) | 获取上次保存的时间（本地时区）。 |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | 获取上次保存的通用时间。 |
| [getLines()](#getLines--) | 表示文档行数的估计值。 |
| [getLinksUpToDate()](#getLinksUpToDate--) | 指示文档中的超链接是否是最新的。 |
| [getManager()](#getManager--) | 获取 manager 属性。 |
| [getNameOfApplication()](#getNameOfApplication--) | 获取应用程序的名称。 |
| [getPages()](#getPages--) | 表示文档页数的估计值。 |
| [getParagraphs()](#getParagraphs--) | 表示文档段落数的估计值。 |
| [getRevisionNumber()](#getRevisionNumber--) | 获取文档修订号。 |
| [getScaleCrop()](#getScaleCrop--) | 指示文档缩略图的显示模式。 |
| [getSubject()](#getSubject--) | 获取文档主题。 |
| [getTemplate()](#getTemplate--) | 获取文档模板的信息名称。 |
| [getTitle()](#getTitle--) | 获取文档标题。 |
| [getTotalEditingTime()](#getTotalEditingTime--) | 获取以分钟为单位的总编辑时间。 |
| [getVersion()](#getVersion--) | 表示创建文档的应用程序的版本号。 |
| [getWords()](#getWords--) | 表示文档中单词数量的估计值。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [indexOf(String name)](#indexOf-java.lang.String-) | 根据名称获取属性的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | 从集合中移除具有指定名称的属性。 |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的属性。 |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置文档作者的姓名。 |
| [setBytes(int value)](#setBytes-int-) | 表示文档中字节数的估计值。 |
| [setCategory(String value)](#setCategory-java.lang.String-) | 设置文档的类别。 |
| [setCharacters(int value)](#setCharacters-int-) | 表示文档中字符数的估计值。 |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | 表示文档中字符数（包括空格）的估计值。 |
| [setComments(String value)](#setComments-java.lang.String-) | 设置文档的注释。 |
| [setCompany(String value)](#setCompany-java.lang.String-) | 设置公司属性。 |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | 设置文档的内容状态。 |
| [setContentType(String value)](#setContentType-java.lang.String-) | 设置文档的内容类型。 |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | 设置文档创建日期（本地时区）。 |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | 设置文档创建的 UTC 时间。 |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | 表示文件的版本。 |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | 设置 hyperlinkbase 属性。 |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | 设置文档关键字。 |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | 设置文档的语言。 |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | 设置文档上次打印日期（本地时区）。 |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | 设置文档上次打印的 UTC 时间。 |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | 设置最后一位作者的姓名。 |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | 设置上次保存时间（本地时区）。 |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | 设置上次保存的 UTC 时间。 |
| [setLines(int value)](#setLines-int-) | 表示文档行数的估计值。 |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | 指示文档中的超链接是否是最新的。 |
| [setManager(String value)](#setManager-java.lang.String-) | 设置 manager 属性。 |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | 设置应用程序的名称。 |
| [setPages(int value)](#setPages-int-) | 表示文档页数的估计值。 |
| [setParagraphs(int value)](#setParagraphs-int-) | 表示文档段落数的估计值。 |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | 设置文档的修订号。 |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | 指示文档缩略图的显示模式。 |
| [setSubject(String value)](#setSubject-java.lang.String-) | 设置文档的主题。 |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | 设置文档模板的信息名称。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 设置文档的标题。 |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | 设置总编辑时间（分钟）。 |
| [setVersion(String value)](#setVersion-java.lang.String-) | 表示创建文档的应用程序的版本号。 |
| [setWords(int value)](#setWords-int-) | 表示文档中单词数量的估计值。 |
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
### clear() {#clear--}
```
public void clear()
```


从 CollectionBase 实例中移除所有对象。

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


如果集合中存在具有指定名称的属性，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

**Returns:**
boolean - 如果属性存在于集合中则为 True；否则为 false。
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
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


通过索引返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 要检索的 [DocumentProperty](../../com.aspose.cells/documentproperty) 的零基索引。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


通过属性名称返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。

**Remarks**

属性的字符串名称对应于可从 中获取的已键入属性的名称。

如果请求的属性在文档中不存在，但属性名称被识别为有效的内置名称，则会创建一个新的  ，将其添加到集合中并返回。新创建的属性会分配默认值（空字符串、零、false 或 DateTime.MinValue，具体取决于内置属性的类型）。

如果请求的属性在文档中不存在且名称未被识别为内置名称，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 要检索的属性的大小写不敏感名称。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


获取文档作者的名称。

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


表示文档中字节数的估计值。

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


获取文档的类别。

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


表示文档中字符数的估计值。

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


表示文档中字符数（包括空格）的估计值。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


获取文档注释。

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


获取公司属性。

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


获取文档的内容状态。

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


获取文档的内容类型。

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


获取文档创建日期（本地时区）。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


获取文档创建的通用时间。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


表示文件的版本。

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


获取 hyperlinkbase 属性。

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


获取文档关键字。

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


获取文档语言。

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


获取文档上次打印的日期（本地时区）。

**Remarks**

如果文档从未打印过，此属性将返回 DateTime.MinValue。

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


获取文档上次打印的通用时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


获取最后作者的姓名。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


获取上次保存的时间（本地时区）。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


获取上次保存的通用时间。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


表示文档行数的估计值。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


指示文档中的超链接是否是最新的。

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


获取 manager 属性。

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


获取应用程序的名称。

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


表示文档页数的估计值。

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


表示文档段落数的估计值。

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


获取文档修订号。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


指示文档缩略图的显示模式。

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


获取文档主题。

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


获取文档模板的信息名称。

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


获取文档标题。

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


获取以分钟为单位的总编辑时间。

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


表示创建文档的应用程序的版本号。

**Remarks**

其格式为 "00.0000"，例如：12.0000。

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


表示文档中单词数量的估计值。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


根据名称获取属性的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

**Returns:**
int - 零基索引。如果未找到则为负值。
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


从集合中移除具有指定名称的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 零基索引。 |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


设置文档作者的姓名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


表示文档中字节数的估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


设置文档的类别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


表示文档中字符数的估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


表示文档中字符数（包括空格）的估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


设置文档的注释。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


设置公司属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


设置文档的内容状态。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


设置文档的内容类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


设置文档创建日期（本地时区）。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


设置文档创建的 UTC 时间。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


表示文件的版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


设置 hyperlinkbase 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


设置文档关键字。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


设置文档的语言。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


设置文档上次打印日期（本地时区）。

**Remarks**

如果文档从未打印过，此属性将返回 DateTime.MinValue。

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


设置文档上次打印的 UTC 时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


设置最后一位作者的姓名。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


设置上次保存时间（本地时区）。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


设置上次保存的 UTC 时间。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


表示文档行数的估计值。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


指示文档中的超链接是否是最新的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


设置 manager 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


设置应用程序的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


表示文档页数的估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


表示文档段落数的估计值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


设置文档的修订号。

**Remarks**

在修改文档时，Aspose.Cells 不会更新此属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


指示文档缩略图的显示模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


设置文档的主题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


设置文档模板的信息名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


设置文档的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


设置总编辑时间（分钟）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


表示创建文档的应用程序的版本号。

**Remarks**

其格式为 "00.0000"，例如：12.0000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


表示文档中单词数量的估计值。

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

