---
title: "GridValidationType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据验证类型。"
type: docs
url: /zh/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

表示数据验证类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | 任意值验证类型。 |
| [BOOLEAN](#BOOLEAN) | TRUE 或 FALSE |
| [CHECK_BOX](#CHECK-BOX) | 将单元格显示为复选框。 |
| [CUSTOM](#CUSTOM) | 自定义验证类型。 |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | 使用正则表达式的自定义验证类型。 |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | 自定义 javascript 函数验证。 |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | 自定义服务器端函数验证。 |
| [DATE](#DATE) | 日期验证类型。 |
| [DATE_TIME](#DATE-TIME) | DateTime（yyyy-MM-dd 或 yyyy-MM-dd hh:mm:ss）。 |
| [DECIMAL](#DECIMAL) | 十进制验证类型。 |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | 显示下拉列表。 |
| [FREE_LIST](#FREE-LIST) | 自由列表验证类型。 |
| [LIST](#LIST) | 列表验证类型。 |
| [TEXT_LENGTH](#TEXT-LENGTH) | 文本长度验证类型。 |
| [TIME](#TIME) | 时间验证类型。 |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | 整数验证类型。 |
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
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


任意值验证类型。

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


TRUE 或 FALSE

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


将单元格显示为复选框。且单元格的值为 True 或 False。

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


自定义验证类型。

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


使用正则表达式的自定义验证类型。

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


自定义 javascript 函数验证。

**Remarks**

使用 ClientValidationFunction 属性指定客户端验证函数的名称。函数应按以下形式声明：
function customValicationFunction(source, value)
参数 "source" 是单元格对象。参数 "value" 是待检查的单元格的字符串值。如果该值有效，函数应返回 true。

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


自定义服务器端函数验证。

**Remarks**

使用 CustomServerFunction 属性来指定服务器端验证。下面是示例代码：
首先定义实现 GridCustomServerValidation 的类，例如 myservervali : GridCustomServerValidation
...... 然后添加验证 var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); 然后设置 ClientValidationFunction 以处理服务器验证失败时的客户端逻辑并返回消息 gv.ClientValidationFunction = "ValidationErrorClientFunction"; 客户端函数应声明如下：function ValidationErrorClientFunction(cell,msg) 请查看演示页面获取详细参考

### DATE {#DATE}
```
public static final int DATE
```


日期验证类型。

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


DateTime（yyyy-MM-dd 或 yyyy-MM-dd hh:mm:ss）。

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


十进制验证类型。

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


显示下拉列表。

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


自由列表验证类型。

### LIST {#LIST}
```
public static final int LIST
```


列表验证类型。

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


文本长度验证类型。

### TIME {#TIME}
```
public static final int TIME
```


时间验证类型。

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


整数验证类型。

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

