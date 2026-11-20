---
title: "FormulaSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Настройки формул и вычислений."
type: docs
url: /ru/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Настройки формул и вычислений.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Указывает, требуется ли приложению выполнить полное вычисление при открытии книги. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений. |
| [getCalculationId()](#getCalculationId--) | Указывает версию движка вычислений, используемого для расчёта значений в книге. |
| [getCalculationMode()](#getCalculationMode--) | Получает режим вычисления книги в MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Указывает, следует ли включить цепочку вычислений для формул. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Указывает, следует ли включить итеративные вычисления для разрешения циклических ссылок. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Указывает, вычисляются ли все формулы каждый раз при запуске вычисления. |
| [getMaxChange()](#getMaxChange--) | Максимальное изменение для разрешения циклической ссылки. |
| [getMaxIteration()](#getMaxIteration--) | Максимальное количество итераций для разрешения циклической ссылки. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Указывает, должна ли точность рассчитанного результата устанавливаться в соответствии с отображаемым при вычислении формул. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Указывает, требуется ли приложению выполнить полное вычисление при открытии книги. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Указывает версию движка вычислений, используемого для расчёта значений в книге. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Устанавливает режим вычисления книги в MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Указывает, следует ли включить цепочку вычислений для формул. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Указывает, следует ли включить итеративные вычисления для разрешения циклических ссылок. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Указывает, вычисляются ли все формулы каждый раз при запуске вычисления. |
| [setMaxChange(double value)](#setMaxChange-double-) | Максимальное изменение для разрешения циклической ссылки. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Максимальное количество итераций для разрешения циклической ссылки. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Указывает, должна ли точность рассчитанного результата устанавливаться в соответствии с отображаемым при вычислении формул. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Указывает, требуется ли приложению выполнить полное вычисление при открытии книги.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке результирующего файла. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически любые формулы в книге, независимо от того, какое значение было установлено для этого свойства.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Указывает версию движка вычислений, используемого для расчёта значений в книге.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В случае ms excel, если значение этого свойства меньше идентификатора движка пересчёта, связанного с приложением, открывающим результирующий файл, приложение пересчитает результаты всех формул в этой рабочей книге сразу после загрузки файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Получает режим вычисления книги в MS Excel.

См. [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какой режим был установлен для этого свойства. Если пользователю необходимо вычислять формулы, пожалуйста, всегда вызывайте методы различных объектов в соответствии с требованием: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Указывает, следует ли включать цепочку вычислений для формул. По умолчанию — false.

**Remarks**

Когда в рабочей книге много формул и пользователю нужно вычислять их повторно, изменяя только небольшую часть, включение цепочки вычислений может улучшить производительность. С другой стороны, если цепочка включена, поддержание её модели требует дополнительной памяти и также требует немного больше процессорного времени для некоторых других операций, таких как изменение значения ячейки или формул. После изменения этого свойства с false на true цепочка вычислений будет проанализирована и построена во время первого вычисления рабочей книги, поэтому требуемое время первого вычисления может быть больше, чем обычное вычисление без цепочки.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Указывает, следует ли включить итеративные вычисления для разрешения циклических ссылок.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Указывает, вычисляются ли все формулы каждый раз при запуске вычисления.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Максимальное изменение для разрешения циклической ссылки.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Максимальное количество итераций для разрешения циклической ссылки.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Указывает, должна ли точность рассчитанного результата устанавливаться в соответствии с отображаемым при вычислении формул.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

Обычно эти пробелы и разрывы строк нужны только для визуального оформления; их сохранение или отсутствие не влияет на вычисленный результат. В целях производительности, если нет особых требований, лучше не сохранять их при обработке формул.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Указывает, требуется ли приложению выполнить полное вычисление при открытии книги.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке результирующего файла. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически любые формулы в книге, независимо от того, какое значение было установлено для этого свойства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Указывает версию движка вычислений, используемого для расчёта значений в книге.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В случае ms excel, если значение этого свойства меньше идентификатора движка пересчёта, связанного с приложением, открывающим результирующий файл, приложение пересчитает результаты всех формул в этой рабочей книге сразу после загрузки файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Устанавливает режим вычисления книги в MS Excel.

См. [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какой режим был установлен для этого свойства. Если пользователю необходимо вычислять формулы, пожалуйста, всегда вызывайте методы различных объектов в соответствии с требованием: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Указывает, следует ли включать цепочку вычислений для формул. По умолчанию — false.

**Remarks**

Когда в рабочей книге много формул и пользователю нужно вычислять их повторно, изменяя только небольшую часть, включение цепочки вычислений может улучшить производительность. С другой стороны, если цепочка включена, поддержание её модели требует дополнительной памяти и также требует немного больше процессорного времени для некоторых других операций, таких как изменение значения ячейки или формул. После изменения этого свойства с false на true цепочка вычислений будет проанализирована и построена во время первого вычисления рабочей книги, поэтому требуемое время первого вычисления может быть больше, чем обычное вычисление без цепочки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Указывает, следует ли включить итеративные вычисления для разрешения циклических ссылок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Указывает, вычисляются ли все формулы каждый раз при запуске вычисления.

**Remarks**

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы, чтобы другие приложения (например, ms excel) могли соответствующим образом реагировать при загрузке и обработке результирующего файла. В целях производительности для большинства пользовательских приложений мы не вычисляем любые формулы в рабочей книге автоматически, независимо от того, какое значение было установлено для этого свойства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


Максимальное изменение для разрешения циклической ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Максимальное количество итераций для разрешения циклической ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Указывает, должна ли точность рассчитанного результата устанавливаться в соответствии с отображаемым при вычислении формул.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

Обычно эти пробелы и разрывы строк нужны только для визуального оформления; их сохранение или отсутствие не влияет на вычисленный результат. В целях производительности, если нет особых требований, лучше не сохранять их при обработке формул.

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

