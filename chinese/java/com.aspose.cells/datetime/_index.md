---
title: "DateTime"
second_title: "Aspose.Cells for Java API 参考"
description: "表示一个时间点，通常表示为日期和时间。"
type: docs
url: /zh/java/com.aspose.cells/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

表示时间点，通常表示为日期和时间。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | 将 DateTime 对象初始化为指定的年、月和日的新实例。 |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | 将 DateTime 对象初始化为指定的年、月、日、小时、分钟和秒的新实例。 |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | 将 DateTime 对象初始化为指定的年、月、日、小时、分钟、秒和毫秒的新实例。 |
| [DateTime(Date date)](#DateTime-java.util.Date-) | 将 DateTime 对象初始化为指定的 Date 对象的新实例。 |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | 将 DateTime 对象初始化为指定的 Calendar 对象的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addDays(double value)](#addDays-double-) | 将指定的天数添加到此实例的值中。 |
| [addHours(double value)](#addHours-double-) | 将指定的小时数添加到此实例的值中。 |
| [addMilliseconds(double value)](#addMilliseconds-double-) | 将指定的毫秒数添加到此实例的值中。 |
| [addMinutes(double value)](#addMinutes-double-) | 将指定的分钟数添加到此实例的值中。 |
| [addMonths(int months)](#addMonths-int-) | 将指定的月份数添加到此实例的值中。 |
| [addSeconds(double value)](#addSeconds-double-) | 将指定的秒数添加到此实例的值中。 |
| [addYears(int value)](#addYears-int-) | 将指定的年数添加到此实例的值中。 |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | 比较此实例的值与指定的 DateTime 值，并返回一个整数，指示此实例是早于、等于还是晚于指定的 DateTime 值。 |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | 将此实例的值与包含指定 DateTime 值的对象进行比较，并返回一个整数，指示此实例是早于、等于还是晚于指定的 DateTime 值。 |
| [equals(Object value)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | 获取此实例表示的月份中的天数。 |
| [getDayOfWeek()](#getDayOfWeek--) | 获取此实例表示的星期几。 |
| [getDayOfYear()](#getDayOfYear--) | 获取此实例表示的年份中的天数。 |
| [getHour()](#getHour--) | 获取此实例表示的日期的小时部分。 |
| [getMillisecond()](#getMillisecond--) | 获取此实例表示的日期的毫秒部分。 |
| [getMinute()](#getMinute--) | 获取此实例表示的日期的分钟部分。 |
| [getMonth()](#getMonth--) | 获取此实例表示的日期的月份部分。 |
| [getNow()](#getNow--) | 获取一个 DateTime 对象，该对象设置为此计算机的当前日期和时间，以本地时间表示。 |
| [getSecond()](#getSecond--) | 获取此实例表示的日期的秒数部分。 |
| [getYear()](#getYear--) | 获取此实例表示的日期的年份部分。 |
| [hashCode()](#hashCode--) | 返回此实例的哈希码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | 将当前 DateTime 对象的值转换为 Calendar 对象。 |
| [toDate()](#toDate--) | 将当前 DateTime 对象的值转换为 Date 对象。 |
| [toLocalTime()](#toLocalTime--) | 将当前 DateTime 对象的值转换为本地时间。 |
| [toString()](#toString--) | 将当前 DateTime 对象的值转换为等效的字符串表示形式。 |
| [toUniversalTime()](#toUniversalTime--) | 将当前 DateTime 对象的值转换为协调世界时 (UTC)。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


将 DateTime 对象初始化为指定的年、月和日的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 年 | int | 年份（1 到 9999）。 |
| 月 | int | 月份（1 到 12）。 |
| 日 | int | 天数（1 到该月的天数）。 |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


将 DateTime 对象初始化为指定的年、月、日、小时、分钟和秒的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 年 | int | 年份（1 到 9999）。 |
| 月 | int | 月份（1 到 12）。 |
| 日 | int | 天数（1 到该月的天数）。 |
| 小时 | int | 小时（0 到 23）。 |
| 分钟 | int | 分钟（0 到 59）。 |
| 秒 | int | 秒（0 到 59）。 |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


将 DateTime 对象初始化为指定的年、月、日、小时、分钟、秒和毫秒的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 年 | int | 年份（1 到 9999）。 |
| 月 | int | 月份（1 到 12）。 |
| 日 | int | 天数（1 到该月的天数）。 |
| 小时 | int | 小时（0 到 23）。 |
| 分钟 | int | 分钟（0 到 59）。 |
| 秒 | int | 秒（0 到 59）。 |
| 毫秒 | int | 毫秒（0 到 999）。 |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


将 DateTime 对象初始化为指定的 Date 对象的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日期 | java.util.Date | Date 对象 |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


将 DateTime 对象初始化为指定的 Calendar 对象的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cld | java.util.Calendar | Calendar 对象 |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


将指定的天数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 一个包含整数和小数部分的天数。value 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


将指定的小时数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 一个包含整数和小数部分的小时数。value 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


将指定的毫秒数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 一个包含整数和小数部分的毫秒数。value 参数可以为负或为正。请注意，此值会四舍五入到最近的整数。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


将指定的分钟数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 一个包含整数和小数部分的分钟数。value 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


将指定的月份数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 月份 | int | 月份数。months 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


将指定的秒数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 一个包含整数和小数部分的秒数。value 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


将指定的年数添加到此实例的值中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 一个包含整数和小数部分的年数。value 参数可以为负或为正。 |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```


比较此实例的值与指定的 DateTime 值，并返回一个整数，指示此实例是早于、等于还是晚于指定的 DateTime 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | 用于比较的 DateTime 对象。 |

**Returns:**
int - 一个有符号数，指示此实例与 value 参数的相对值。Value Description 小于零 此实例早于 value。零 此实例与 value 相同。大于零 此实例晚于 value。
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


将此实例的值与包含指定 DateTime 值的对象进行比较，并返回一个整数，指示此实例是早于、等于还是晚于指定的 DateTime 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 用于比较的装箱 DateTime 对象，或 null。 |

**Returns:**
int - 一个有符号数，指示此实例与 value 的相对值。Value Description 小于零 此实例早于 value。零 此实例与 value 相同。大于零 此实例晚于 value，或 value 为 null。
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - 如果 value 是 DateTime 的实例并且等于此实例的值，则为 true；否则为 false。
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


获取此实例表示的月份中的天数。

**Returns:**
int - 天组件，取值范围为 1 到 31。
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


获取此实例表示的星期几。

**Returns:**
int - 此 DateTime 值的星期几。
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


获取此实例表示的年份中的天数。

**Returns:**
int - 一年中的天数，取值范围为 1 到 366。
### getHour() {#getHour--}
```
public int getHour()
```


获取此实例表示的日期的小时部分。

**Returns:**
int - 小时组件，取值范围为 0 到 23。
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


获取此实例表示的日期的毫秒部分。

**Returns:**
int - 毫秒组件，取值范围为 0 到 999。
### getMinute() {#getMinute--}
```
public int getMinute()
```


获取此实例表示的日期的分钟部分。

**Returns:**
int - 分钟组件，取值范围为 0 到 59。
### getMonth() {#getMonth--}
```
public int getMonth()
```


获取此实例表示的日期的月份部分。

**Returns:**
int - 月份组件，取值范围为 1 到 12。
### getNow() {#getNow--}
```
public static DateTime getNow()
```


获取一个 DateTime 对象，该对象设置为此计算机的当前日期和时间，以本地时间表示。

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


获取此实例表示的日期的秒数部分。

**Returns:**
int - 秒数，取值范围为 0 到 59。
### getYear() {#getYear--}
```
public int getYear()
```


获取此实例表示的日期的年份部分。

**Returns:**
int - 年份，取值范围为 1 到 9999。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回此实例的哈希码。

**Returns:**
int - 32 位有符号整数哈希码。
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


将当前 DateTime 对象的值转换为 Calendar 对象。

**Returns:**
java.util.Calendar - Calendar 对象
### toDate() {#toDate--}
```
public Date toDate()
```


将当前 DateTime 对象的值转换为 Date 对象。

**Returns:**
java.util.Date - Date 对象
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


将当前 DateTime 对象的值转换为本地时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


将当前 DateTime 对象的值转换为等效的字符串表示形式。

**Returns:**
java.lang.String - 当前 DateTime 对象值的字符串表示。
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


将当前 DateTime 对象的值转换为协调世界时 (UTC)。

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

