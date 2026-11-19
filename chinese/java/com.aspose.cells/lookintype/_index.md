---
title: "LookInType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示查找类型。"
type: docs
url: /zh/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

表示查找类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [COMMENTS](#COMMENTS) | 仅从单元格的批注中查找对象。 |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | 仅从单元格的格式化值([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) 查找对象。 |
| [FORMULAS](#FORMULAS) | 如果单元格是公式，则从公式([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) 中查找目标对象；否则从单元格的原始值（与 [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES) 相同）中查找。 |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | 忽略非公式的单元格。 |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | 仅从单元格的原始值查找对象。 |
| [VALUES](#VALUES) | 从单元格的原始值([Cell.getValue()](../../com.aspose.cells/cell\#getValue--))和格式化值([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--))中查找对象。 |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | 忽略公式单元格。 |
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
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


仅从单元格的批注中查找对象。忽略没有批注的单元格。

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


仅从单元格的格式化值([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) 查找对象。

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


如果单元格是公式，则从公式([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) 中查找目标对象；否则从单元格的原始值（与 [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES) 相同）中查找。

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


忽略非公式的单元格。对于公式单元格，从公式([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) 中查找目标对象。

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


仅从单元格的原始值查找对象。

### VALUES {#VALUES}
```
public static final int VALUES
```


从单元格的原始值([Cell.getValue()](../../com.aspose.cells/cell\#getValue--))和格式化值([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--))中查找对象。

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


忽略公式单元格。对于非公式的单元格，其行为与 [VALUES](../../com.aspose.cells/lookintype\#VALUES) 相同。

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

