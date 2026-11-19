---
title: "GridAbstractCalculationEngine"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。"
type: docs
url: /zh/java/com.aspose.gridweb/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridweb.GridCalculationData-) | 使用给定数据计算一个函数。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridweb.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


使用给定数据计算一个函数。

**Remarks**

用户应为给定数据设置所有函数（包括 Excel 原生函数）的计算值，以便在此实现中自行计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridweb/gridcalculationdata) | 计算函数所需的数据，例如函数名称、参数等。 |

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

