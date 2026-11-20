---
title: "CalculationOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры вычисления."
type: docs
url: /ru/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Представляет параметры вычисления.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | Размер стека для рекурсивного вычисления ячеек. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Монитор для отслеживания пользователем прогресса вычисления формул. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Пользовательский движок вычисления формул для расширения движка вычислений по умолчанию в Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Указывает источники данных для внешних ссылок, используемых в формулах. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Указывает стратегию обработки точности вычислений. |
| [getRecursive()](#getRecursive--) | Указывает, следует ли рекурсивно вычислять зависимые ячейки при вычислении одной ячейки, если она зависит от других ячеек. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Указывает, указал ли пользователь явно поведение обновления формул динамических массивов перед вычислением указанных формул. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Размер стека для рекурсивного вычисления ячеек. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Монитор для отслеживания пользователем прогресса вычисления формул. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Пользовательский движок вычисления формул для расширения движка вычислений по умолчанию в Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Указывает источники данных для внешних ссылок, используемых в формулах. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Указывает стратегию обработки точности вычислений. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Указывает, следует ли рекурсивно вычислять зависимые ячейки при вычислении одной ячейки, если она зависит от других ячеек. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
```


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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Размер стека для рекурсивного вычисления ячеек. Значение по умолчанию — 200.

**Remarks**

Когда требуется рекурсивно вычислять большое количество ячеек в дереве зависимостей, в процессе вычисления может возникнуть StackOverflowException. В этом случае пользователь должен указать меньшее значение для этого свойства. Для такой ситуации пользователь должен определить подходящее значение свойства в соответствии с реальными формулами и данными. Однако слишком маленькое значение может привести к снижению производительности вычисления формул, а значение меньше 2 сделает невозможным вычисление формулы, зависящей от другой. Поэтому если указанное значение меньше 2, оно будет сброшено до 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Монитор для отслеживания пользователем прогресса вычисления формул.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. Для функций, таких как CHAR, CODE, полученный результат зависит от региональных настроек и кодировки по умолчанию среды. С помощью этого свойства пользователь может указать правильную кодировку, используемую этими функциями, чтобы получить ожидаемый результат.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


Пользовательский движок вычисления формул для расширения движка вычислений по умолчанию в Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. Ошибкой может быть неподдерживаемая функция, внешние ссылки и т.д. Значение по умолчанию — true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Указывает источники данных для внешних ссылок, используемых в формулах.

**Remarks**

Как и в случае [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), здесь вы можете указать источники данных для внешних ссылок, используемых в формулах, которые необходимо вычислить, особенно для тех, которые используются в функции INDIRECT. Такие внешние ссылки, используемые в функции INDIRECT, не считаются частью внешних ссылок книги и не могут быть обновлены с помощью [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). Соответствие этих книг внешним ссылкам определяется методами [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) и [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Поэтому, пожалуйста, убедитесь, что [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) указано с правильным значением (обычно оно должно совпадать с соответствующим [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) для каждой книги, чтобы они могли быть связаны как ожидается.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Указывает стратегию обработки точности вычислений.

Смотрите [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Указывает, следует ли рекурсивно вычислять зависимые ячейки при расчёте одной ячейки, если она зависит от других ячеек. Значение по умолчанию — true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул.

**Remarks**

Если это свойство было указано явно, то указанное значение будет использоваться для определения, следует ли обновлять формулы динамических массивов. В противном случае ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) возвращает false), значение по умолчанию зависит от типа формул, которые необходимо вычислять: для вычисления формул книги, например [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), это свойство считается true. Для других случаев, например [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) или [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), это свойство считается false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Указывает, указал ли пользователь явно поведение обновления формул динамических массивов перед вычислением указанных формул.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


Размер стека для рекурсивного вычисления ячеек. Значение по умолчанию — 200.

**Remarks**

Когда требуется рекурсивно вычислять большое количество ячеек в дереве зависимостей, в процессе вычисления может возникнуть StackOverflowException. В этом случае пользователь должен указать меньшее значение для этого свойства. Для такой ситуации пользователь должен определить подходящее значение свойства в соответствии с реальными формулами и данными. Однако слишком маленькое значение может привести к снижению производительности вычисления формул, а значение меньше 2 сделает невозможным вычисление формулы, зависящей от другой. Поэтому если указанное значение меньше 2, оно будет сброшено до 2.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Монитор для отслеживания пользователем прогресса вычисления формул.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. Для функций, таких как CHAR, CODE, полученный результат зависит от региональных настроек и кодировки по умолчанию среды. С помощью этого свойства пользователь может указать правильную кодировку, используемую этими функциями, чтобы получить ожидаемый результат.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Пользовательский движок вычисления формул для расширения движка вычислений по умолчанию в Aspose.Cells.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. Ошибкой может быть неподдерживаемая функция, внешние ссылки и т.д. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Указывает источники данных для внешних ссылок, используемых в формулах.

**Remarks**

Как и в случае [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), здесь вы можете указать источники данных для внешних ссылок, используемых в формулах, которые необходимо вычислить, особенно для тех, которые используются в функции INDIRECT. Такие внешние ссылки, используемые в функции INDIRECT, не считаются частью внешних ссылок книги и не могут быть обновлены с помощью [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). Соответствие этих книг внешним ссылкам определяется методами [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) и [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Поэтому, пожалуйста, убедитесь, что [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) указано с правильным значением (обычно оно должно совпадать с соответствующим [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) для каждой книги, чтобы они могли быть связаны как ожидается.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Указывает стратегию обработки точности вычислений.

Смотрите [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Указывает, следует ли рекурсивно вычислять зависимые ячейки при расчёте одной ячейки, если она зависит от других ячеек. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул.

**Remarks**

Если это свойство было указано явно, то указанное значение будет использоваться для определения, следует ли обновлять формулы динамических массивов. В противном случае ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) возвращает false), значение по умолчанию зависит от типа формул, которые необходимо вычислять: для вычисления формул книги, например [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), это свойство считается true. Для других случаев, например [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) или [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), это свойство считается false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

