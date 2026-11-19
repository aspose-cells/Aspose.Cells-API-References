---
title: "DigitalSignatureCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "提供附加在文档上的数字签名集合。"
type: docs
url: /zh/java/com.aspose.cells/digitalsignaturecollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DigitalSignatureCollection implements Iterable
```

提供附加在文档上的数字签名集合。

**Example**

下面的示例展示了如何验证数字签名。

```
         //workbook from a signed source file
         Workbook signedWorkbook = new Workbook("signedFile.xlsx");
         //wb.IsDigitallySigned is true when the workbook is signed already.
         System.out.println(signedWorkbook.isDigitallySigned());
         //get digitalSignature collection from workbook
         DigitalSignatureCollection existingDsc = signedWorkbook.getDigitalSignature();
         for (DigitalSignature existingDs : (Iterable<DigitalSignature>) existingDsc)
         {
             System.out.println(existingDs.getComments());
             System.out.println(existingDs.getSignTime());
             System.out.println(existingDs.isValid());
         }
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DigitalSignatureCollection()](#DigitalSignatureCollection--) | DigitalSignatureCollection 的构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(DigitalSignature digitalSignature)](#add-com.aspose.cells.DigitalSignature-) | 向 DigitalSignatureCollection 添加一个签名。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取 DigitalSignatureCollection 的枚举器，该枚举器允许遍历集合。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignatureCollection() {#DigitalSignatureCollection--}
```
public DigitalSignatureCollection()
```


DigitalSignatureCollection 的构造函数。

### add(DigitalSignature digitalSignature) {#add-com.aspose.cells.DigitalSignature-}
```
public void add(DigitalSignature digitalSignature)
```


向 DigitalSignatureCollection 添加一个签名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | 集合中的数字签名。 |

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
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取 DigitalSignatureCollection 的枚举器，该枚举器允许遍历集合。

**Returns:**
java.util.Iterator - 用于迭代的枚举器。
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

