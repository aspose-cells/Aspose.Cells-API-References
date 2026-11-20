---
title: "GridAbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells."
type: docs
url: /ru/java/com.aspose.gridjs/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells.

**Remarks**

Пользователь не должен изменять любую часть Workbook напрямую в этой реализации (за исключением вычисленного результата пользовательской функции, который можно задать через свойство GridCalculationData.CalculatedValue). В противном случае могут возникнуть неожиданные результаты или Exception. Если пользователю необходимо изменить другие данные, отличные от вычисленного результата, в реализации для некоторых пользовательских функций, например изменить формулу ячейки, стиль и т.д., пользователь должен собрать эти данные в этой реализации и изменить их вне области вычисления формул.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridjs.GridCalculationData-) | Вычисляет одну функцию с заданными данными. |
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


### calculate(GridCalculationData data) {#calculate-com.aspose.gridjs.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Вычисляет одну функцию с заданными данными.

**Remarks**

Пользователь должен установить вычисленное значение для заданных данных для всех функций (включая встроенные функции Excel), которые он хочет вычислять самостоятельно в этой реализации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridjs/gridcalculationdata) | Требуемые данные для вычисления функции, такие как имя функции, параметры и т.д. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

