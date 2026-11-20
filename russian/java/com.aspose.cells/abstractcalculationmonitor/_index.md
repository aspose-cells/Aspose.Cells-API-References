---
title: "AbstractCalculationMonitor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул."
type: docs
url: /ru/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Реализуйте этот метод для выполнения действий после вычисления ячейки. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Реализуйте этот метод для выполнения действий перед вычислением ячейки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Получает новое вычисленное значение ячейки. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Получает старое значение вычисленной ячейки. |
| [getValueChanged()](#getValueChanged--) | Указывает, изменилось ли значение ячейки после вычисления. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Реализуйте этот метод для выполнения действий при вычислении формул с круговыми ссылками. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Реализуйте этот метод для выполнения действий после вычисления ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа, к которому относится ячейка. |
| rowIndex | int | Индекс строки ячейки |
| colIndex | int | Индекс столбца ячейки |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Реализуйте этот метод для выполнения действий перед вычислением ячейки.

**Remarks**

Для ячеек в массивных формулах этот метод может не быть выполнен, поскольку такие ячейки обычно вычисляются вместе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа, к которому относится ячейка. |
| rowIndex | int | Индекс строки ячейки |
| colIndex | int | Индекс столбца ячейки |

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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Получает новое вычисленное значение ячейки. Должно использоваться только в [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Получает старое значение вычисленной ячейки. Должно использоваться только в [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) и [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Указывает, было ли значение ячейки изменено после вычисления. Должно использоваться только в [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
boolean
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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Реализуйте этот метод для выполнения действий при вычислении формул с круговыми ссылками.

**Remarks**

В реализации пользователь также может задать ожидаемое значение как результат вычисления для части/всех этих ячеек, чтобы движок формул не вычислял их рекурсивно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator с элементами [CalculationCell](../../com.aspose.cells/calculationcell), представляющими ячейки, зависящие от круговых ссылок. |

**Returns:**
boolean - Нужно ли движку формул вычислять эти ячейки в круговом режиме после этого вызова. True, чтобы позволить движку формул продолжить вычисление для них. False, чтобы движку формул просто пометить эти ячейки как Calculated.
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

