---
title: "DocumentProperty"
second_title: "Aspose.Cells for Java API 参考"
description: "表示自定义或内置的文档属性。"
type: docs
url: /zh/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

表示自定义或内置的文档属性。

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | 返回属性的名称。 |
| [getSource()](#getSource--) | 链接的内容源。 |
| [getType()](#getType--) | 获取属性的数据类型。 |
| [getValue()](#getValue--) | 获取属性的值。 |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | 如果此属性在 OLE2 存储中没有名称，并且仅为公共 API 生成了唯一名称，则返回 true。 |
| [isLinkedToContent()](#isLinkedToContent--) | 指示此属性是否链接到内容 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置属性的值。 |
| [toBool()](#toBool--) | 以 bool 形式返回属性值。 |
| [toDateTime()](#toDateTime--) | 以本地时区的 DateTime 形式返回属性值。 |
| [toDouble()](#toDouble--) | 以 double 形式返回属性值。 |
| [toInt()](#toInt--) | 以 integer 形式返回属性值。 |
| [toString()](#toString--) | 以字符串形式返回属性值。 |
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


返回属性的名称。

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


链接的内容源。

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


获取属性的数据类型。

参见 [PropertyType](../../com.aspose.cells/propertytype)。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


获取属性的值。

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


如果此属性在 OLE2 存储中没有名称，并且仅为公共 API 生成了唯一名称，则返回 true。

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


指示此属性是否链接到内容

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




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置属性的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


以 bool 形式返回属性值。

**Remarks**

如果属性类型不是 PropertyType.Boolean，则抛出异常。

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


以本地时区的 DateTime 形式返回属性值。

**Remarks**

如果属性类型不是 PropertyType.Date，则抛出异常。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


以 double 形式返回属性值。

**Remarks**

如果属性类型不是 PropertyType.Float，则抛出异常。

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


以 integer 形式返回属性值。

**Remarks**

如果属性类型不是 PropertyType.Number，则抛出异常。

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


以字符串形式返回属性值。

**Remarks**

使用 Object.ToString() 将数字属性转换为字符串。将布尔属性转换为 "Y" 或 "N"。将日期属性转换为短日期字符串。

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

