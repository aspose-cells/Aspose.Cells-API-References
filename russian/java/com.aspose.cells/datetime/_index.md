---
title: "DateTime"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет момент времени, обычно выраженный как дата и время суток."
type: docs
url: /ru/java/com.aspose.cells/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Представляет момент времени, обычно выраженный как дата и время суток.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем и днём. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем, днём, часом, минутой и секундой. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем, днём, часом, минутой, секундой и миллисекундой. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Инициализирует новый экземпляр объекта DateTime с указанным объектом Date. |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Инициализирует новый экземпляр объекта DateTime с указанным объектом Calendar. |
## Методы

| Метод | Описание |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Добавляет указанное количество дней к значению этого экземпляра. |
| [addHours(double value)](#addHours-double-) | Добавляет указанное количество часов к значению этого экземпляра. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Добавляет указанное количество миллисекунд к значению этого экземпляра. |
| [addMinutes(double value)](#addMinutes-double-) | Добавляет указанное количество минут к значению этого экземпляра. |
| [addMonths(int months)](#addMonths-int-) | Добавляет указанное количество месяцев к значению этого экземпляра. |
| [addSeconds(double value)](#addSeconds-double-) | Добавляет указанное количество секунд к значению этого экземпляра. |
| [addYears(int value)](#addYears-int-) | Добавляет указанное количество лет к значению этого экземпляра. |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | Сравнивает значение этого экземпляра с указанным значением DateTime и возвращает целое число, указывающее, является ли этот экземпляр более ранним, равным или более поздним, чем указанное значение DateTime. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Сравнивает значение этого экземпляра с указанным объектом, содержащим значение DateTime, и возвращает целое число, указывающее, является ли этот экземпляр более ранним, равным или более поздним, чем указанное значение DateTime. |
| [equals(Object value)](#equals-java.lang.Object-) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Возвращает день месяца, представленный этим экземпляром. |
| [getDayOfWeek()](#getDayOfWeek--) | Возвращает день недели, представленный этим экземпляром. |
| [getDayOfYear()](#getDayOfYear--) | Возвращает день года, представленный этим экземпляром. |
| [getHour()](#getHour--) | Возвращает компонент часа даты, представленный этим экземпляром. |
| [getMillisecond()](#getMillisecond--) | Возвращает компонент миллисекунд даты, представленный этим экземпляром. |
| [getMinute()](#getMinute--) | Возвращает компонент минут даты, представленный этим экземпляром. |
| [getMonth()](#getMonth--) | Возвращает компонент месяца даты, представленный этим экземпляром. |
| [getNow()](#getNow--) | Возвращает объект DateTime, установленный на текущие дату и время этого компьютера, выраженный как локальное время. |
| [getSecond()](#getSecond--) | Возвращает компонент секунд даты, представленный этим экземпляром. |
| [getYear()](#getYear--) | Возвращает компонент года даты, представленный этим экземпляром. |
| [hashCode()](#hashCode--) | Возвращает хеш-код этого экземпляра. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Преобразует значение текущего объекта DateTime в объект Calendar. |
| [toDate()](#toDate--) | Преобразует значение текущего объекта DateTime в объект Date. |
| [toLocalTime()](#toLocalTime--) | Преобразует значение текущего объекта DateTime во локальное время. |
| [toString()](#toString--) | Преобразует значение текущего объекта DateTime в его эквивалентное строковое представление. |
| [toUniversalTime()](#toUniversalTime--) | Преобразует значение текущего объекта DateTime в координированное всемирное время (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем и днём.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| год | int | Год (от 1 до 9999). |
| месяц | int | Месяц (от 1 до 12). |
| день | int | День (от 1 до количества дней в месяце). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем, днём, часом, минутой и секундой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| год | int | Год (от 1 до 9999). |
| месяц | int | Месяц (от 1 до 12). |
| день | int | День (от 1 до количества дней в месяце). |
| час | int | Часы (от 0 до 23). |
| минута | int | Минуты (от 0 до 59). |
| секунда | int | Секунды (от 0 до 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Инициализирует новый экземпляр объекта DateTime с указанными годом, месяцем, днём, часом, минутой, секундой и миллисекундой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| год | int | Год (от 1 до 9999). |
| месяц | int | Месяц (от 1 до 12). |
| день | int | День (от 1 до количества дней в месяце). |
| час | int | Часы (от 0 до 23). |
| минута | int | Минуты (от 0 до 59). |
| секунда | int | Секунды (от 0 до 59). |
| миллисекунда | int | Миллисекунды (от 0 до 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Инициализирует новый экземпляр объекта DateTime с указанным объектом Date.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| дата | java.util.Date | Объект Date |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Инициализирует новый экземпляр объекта DateTime с указанным объектом Calendar.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cld | java.util.Calendar | Объект Calendar |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Добавляет указанное количество дней к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double | Число целых и дробных дней. Параметр value может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Добавляет указанное количество часов к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double | Число целых и дробных часов. Параметр value может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Добавляет указанное количество миллисекунд к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double | Число целых и дробных миллисекунд. Параметр value может быть отрицательным или положительным. Обратите внимание, что это значение округляется до ближайшего целого. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Добавляет указанное количество минут к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double | Число целых и дробных минут. Параметр value может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Добавляет указанное количество месяцев к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| месяцы | int | Число месяцев. Параметр months может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Добавляет указанное количество секунд к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double | Число целых и дробных секунд. Параметр value может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Добавляет указанное количество лет к значению этого экземпляра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int | Число лет. Параметр value может быть отрицательным или положительным. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```


Сравнивает значение этого экземпляра с указанным значением DateTime и возвращает целое число, указывающее, является ли этот экземпляр более ранним, равным или более поздним, чем указанное значение DateTime.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | Объект DateTime для сравнения. |

**Returns:**
int - Подписное число, указывающее относительные значения этого экземпляра и параметра value. Описание значения: Меньше нуля — этот экземпляр раньше value. Ноль — этот экземпляр равен value. Больше нуля — этот экземпляр позже value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Сравнивает значение этого экземпляра с указанным объектом, содержащим значение DateTime, и возвращает целое число, указывающее, является ли этот экземпляр более ранним, равным или более поздним, чем указанное значение DateTime.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Упакованный объект DateTime для сравнения или null. |

**Returns:**
int - Подписное число, указывающее относительные значения этого экземпляра и value. Описание значения: Меньше нуля — этот экземпляр раньше value. Ноль — этот экземпляр равен value. Больше нуля — этот экземпляр позже value, или value равно null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object | Объект для сравнения с этим экземпляром. |

**Returns:**
boolean - true, если value является экземпляром DateTime и равен значению этого экземпляра; иначе false.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDay() {#getDay--}
```
public int getDay()
```


Возвращает день месяца, представленный этим экземпляром.

**Returns:**
int - Компонент дня, выраженный значением от 1 до 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Возвращает день недели, представленный этим экземпляром.

**Returns:**
int - День недели значения DateTime.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Возвращает день года, представленный этим экземпляром.

**Returns:**
int - День года, выраженный значением от 1 до 366.
### getHour() {#getHour--}
```
public int getHour()
```


Возвращает компонент часа даты, представленный этим экземпляром.

**Returns:**
int - Компонент часа, выраженный значением от 0 до 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Возвращает компонент миллисекунд даты, представленный этим экземпляром.

**Returns:**
int - Компонент миллисекунд, выраженный значением от 0 до 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Возвращает компонент минут даты, представленный этим экземпляром.

**Returns:**
int - Компонент минут, выраженный значением от 0 до 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Возвращает компонент месяца даты, представленный этим экземпляром.

**Returns:**
int - Компонент месяца, выраженный значением от 1 до 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Возвращает объект DateTime, установленный на текущие дату и время этого компьютера, выраженный как локальное время.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Возвращает компонент секунд даты, представленный этим экземпляром.

**Returns:**
int - Секунды, от 0 до 59.
### getYear() {#getYear--}
```
public int getYear()
```


Возвращает компонент года даты, представленный этим экземпляром.

**Returns:**
int - Год, от 1 до 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Возвращает хеш-код этого экземпляра.

**Returns:**
int - 32-битный подписный целочисленный хеш-код.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toCalendar() {#toCalendar--}
```
public Calendar toCalendar()
```


Преобразует значение текущего объекта DateTime в объект Calendar.

**Returns:**
java.util.Calendar - объект Calendar
### toDate() {#toDate--}
```
public Date toDate()
```


Преобразует значение текущего объекта DateTime в объект Date.

**Returns:**
java.util.Date - объект Date
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Преобразует значение текущего объекта DateTime во локальное время.

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Преобразует значение текущего объекта DateTime в его эквивалентное строковое представление.

**Returns:**
java.lang.String - Строковое представление значения текущего объекта DateTime.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Преобразует значение текущего объекта DateTime в координированное всемирное время (UTC).

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of UTC
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

