---
title: "CalculationPrecisionStrategy"
second_title: "Справочник API Aspose.Cells for Java"
description: "Перечисляет стратегии обработки точности вычислений."
type: docs
url: /ru/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Перечисляет стратегии обработки точности вычислений. Из‑за проблемы точности арифметики с плавающей точкой IEEE 754 некоторые "на вид простые" формулы могут вычисляться не так, как ожидается. Например формула "=-0.45+0.43+0.02", при прямом вычислении операндов оператором '+' результат не равен нулю. Для такого рода проблем точности некоторые специальные стратегии могут дать ожидаемый результат.
## Поля

| Поле | Описание |
| --- | --- |
| [DECIMAL](#DECIMAL) | Использует десятичные числа в качестве операндов, когда это возможно. |
| [NONE](#NONE) | Не применена стратегия при вычислении. |
| [ROUND](#ROUND) | Округляет результат вычисления в соответствии со значимыми цифрами. |
## Методы

| Метод | Описание |
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
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Использует тип decimal в качестве операндов, когда это возможно. Наименее эффективно по производительности.

### NONE {#NONE}
```
public static final int NONE
```


Не применена стратегия при вычислении. При расчёте просто используйте исходное значение double в качестве операнда и возвращайте результат напрямую. Наиболее эффективно по производительности и применимо в большинстве случаев.

### ROUND {#ROUND}
```
public static final int ROUND
```


Округляет результат вычисления в соответствии со значимыми цифрами.

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

