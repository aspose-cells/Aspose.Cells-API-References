---
title: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示全局化设置。"
type: docs
url: /zh/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

表示全局化设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | 根据特定的排序规则比较两个字符串值。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | 根据特定的排序规则将字符串转换为可比较的对象。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


根据特定的排序规则比较两个字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| v1 | java.lang.String | 第一个字符串 |
| v2 | java.lang.String | 第二个字符串 |
| ignoreCase | boolean | 比较值时是否忽略大小写 |

**Returns:**
int - 表示两个比较对象之间词法关系的整数
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


根据特定的排序规则将字符串转换为可比较的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| v | java.lang.String | 字符串值需要与其他值进行比较。 |
| ignoreCase | boolean | 比较值时是否忽略大小写 |

**Returns:**
java.lang.Comparable - 对象可用于比较或排序字符串值
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

