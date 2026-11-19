---
title: "DateTime"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل لحظة في الزمن عادةً ما تُعبّر عنها كتاريخ ووقت اليوم."
type: docs
url: /ar/java/com.aspose.gridweb/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

يمثل لحظة زمنية، عادةً ما تُعبّر عنها كتاريخ ووقت اليوم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | يُنشئ نسخة جديدة من كائن DateTime للسنة والشهر واليوم المحددين. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | يُنشئ مثيلاً جديدًا لكائن DateTime بالقيم المحددة للسنة والشهر واليوم والساعة والدقيقة والثانية. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | يُنشئ مثيلاً جديدًا لكائن DateTime بالقيم المحددة للسنة والشهر واليوم والساعة والدقيقة والثانية والمللي ثانية. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | يُنشئ مثيلاً جديدًا لكائن DateTime باستخدام كائن Date المحدد |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | يُنشئ مثيلاً جديدًا لكائن DateTime باستخدام كائن Calendar المحدد |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addDays(double value)](#addDays-double-) | يضيف العدد المحدد من الأيام إلى قيمة هذا المثيل. |
| [addHours(double value)](#addHours-double-) | يضيف العدد المحدد من الساعات إلى قيمة هذا المثيل. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | يضيف العدد المحدد من المللي ثانية إلى قيمة هذا المثيل. |
| [addMinutes(double value)](#addMinutes-double-) | يضيف العدد المحدد من الدقائق إلى قيمة هذا المثيل. |
| [addMonths(int months)](#addMonths-int-) | يضيف العدد المحدد من الشهور إلى قيمة هذا المثيل. |
| [addSeconds(double value)](#addSeconds-double-) | يضيف العدد المحدد من الثواني إلى قيمة هذا المثيل. |
| [addYears(int value)](#addYears-int-) | يضيف العدد المحدد من السنوات إلى قيمة هذا المثيل. |
| [compareTo(DateTime value)](#compareTo-com.aspose.gridweb.DateTime-) | يقارن قيمة هذا المثيل بقيمة DateTime محددة ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أسبق أو مساوي أو لاحق للقيمة المحددة من DateTime. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | يقارن قيمة هذا المثيل بكائن محدد يحتوي على قيمة DateTime محددة، ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أسبق أو مساوي أو لاحق للقيمة المحددة من DateTime. |
| [equals(Object value)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لكائن محدد. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | يحصل على يوم الشهر الممثل بهذا المثيل. |
| [getDayOfWeek()](#getDayOfWeek--) | يحصل على يوم الأسبوع الممثل بهذا المثيل. |
| [getDayOfYear()](#getDayOfYear--) | يحصل على يوم السنة الممثل بهذا المثيل. |
| [getHour()](#getHour--) | يحصل على مكوّن الساعة من التاريخ الممثل بهذا المثيل. |
| [getMillisecond()](#getMillisecond--) | يحصل على مكوّن المللي ثانية من التاريخ الممثل بهذا المثيل. |
| [getMinute()](#getMinute--) | يحصل على مكوّن الدقيقة من التاريخ الممثل بهذا المثيل. |
| [getMonth()](#getMonth--) | يحصل على مكوّن الشهر من التاريخ الممثل بهذا المثيل. |
| [getNow()](#getNow--) | يحصل على كائن DateTime مضبوط على التاريخ والوقت الحاليين على هذا الحاسوب، معبرًا عنهما بالتوقيت المحلي. |
| [getSecond()](#getSecond--) | يحصل على مكوّن الثواني من التاريخ الممثل بهذا المثيل. |
| [getYear()](#getYear--) | يحصل على مكوّن السنة من التاريخ الممثل بهذا المثيل. |
| [hashCode()](#hashCode--) | يعيد رمز التجزئة لهذا المثيل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | يحوِّل قيمة كائن DateTime الحالي إلى كائن Calendar. |
| [toDate()](#toDate--) | يحوِّل قيمة كائن DateTime الحالي إلى كائن Date. |
| [toLocalTime()](#toLocalTime--) | يحوِّل قيمة كائن DateTime الحالي إلى الوقت المحلي. |
| [toString()](#toString--) | يحوِّل قيمة كائن DateTime الحالي إلى تمثيله النصي المكافئ. |
| [toUniversalTime()](#toUniversalTime--) | يحوِّل قيمة كائن DateTime الحالي إلى الوقت العالمي المنسق (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


يُنشئ نسخة جديدة من كائن DateTime للسنة والشهر واليوم المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| سنة | int | السنة (من 1 إلى 9999). |
| شهر | int | الشهر (من 1 إلى 12). |
| يوم | int | اليوم (من 1 إلى عدد الأيام في الشهر). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


يُنشئ مثيلاً جديدًا لكائن DateTime بالقيم المحددة للسنة والشهر واليوم والساعة والدقيقة والثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| سنة | int | السنة (من 1 إلى 9999). |
| شهر | int | الشهر (من 1 إلى 12). |
| يوم | int | اليوم (من 1 إلى عدد الأيام في الشهر). |
| ساعة | int | الساعات (من 0 إلى 23). |
| دقيقة | int | الدقائق (من 0 إلى 59). |
| ثانية | int | الثواني (من 0 إلى 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


يُنشئ مثيلاً جديدًا لكائن DateTime بالقيم المحددة للسنة والشهر واليوم والساعة والدقيقة والثانية والمللي ثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| سنة | int | السنة (من 1 إلى 9999). |
| شهر | int | الشهر (من 1 إلى 12). |
| يوم | int | اليوم (من 1 إلى عدد الأيام في الشهر). |
| ساعة | int | الساعات (من 0 إلى 23). |
| دقيقة | int | الدقائق (من 0 إلى 59). |
| ثانية | int | الثواني (من 0 إلى 59). |
| ميلي ثانية | int | الميلي الثانية (من 0 إلى 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


يُنشئ مثيلاً جديدًا لكائن DateTime باستخدام كائن Date المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تاريخ | java.util.Date | كائن Date |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


يُنشئ مثيلاً جديدًا لكائن DateTime باستخدام كائن Calendar المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cld | java.util.Calendar | كائن Calendar |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


يضيف العدد المحدد من الأيام إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الأيام الكاملة والجزئية. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


يضيف العدد المحدد من الساعات إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الساعات الكاملة والجزئية. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


يضيف العدد المحدد من المللي ثانية إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الميلي ثانية الكاملة والجزئية. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. لاحظ أن هذه القيمة تُقرب إلى أقرب عدد صحيح. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


يضيف العدد المحدد من الدقائق إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الدقائق الكاملة والجزئية. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


يضيف العدد المحدد من الشهور إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أشهر | int | عدد من الأشهر. يمكن أن يكون معامل الأشهر سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


يضيف العدد المحدد من الثواني إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | عدد من الثواني الكاملة والجزئية. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


يضيف العدد المحدد من السنوات إلى قيمة هذا المثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد من السنوات. يمكن أن يكون معامل القيمة سالبًا أو موجبًا. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.gridweb.DateTime-}
```
public int compareTo(DateTime value)
```


يقارن قيمة هذا المثيل بقيمة DateTime محددة ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أسبق أو مساوي أو لاحق للقيمة المحددة من DateTime.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.gridweb/datetime) | كائن DateTime للمقارنة. |

**Returns:**
int - رقم موقع يشير إلى القيم النسبية لهذه المثيلة ومعامل القيمة. الوصف القيمة أقل من الصفر هذه المثيلة أقدم من القيمة. صفر هذه المثيلة هي نفسها القيمة. أكبر من الصفر هذه المثيلة أحدث من القيمة.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


يقارن قيمة هذا المثيل بكائن محدد يحتوي على قيمة DateTime محددة، ويعيد عددًا صحيحًا يشير إلى ما إذا كان هذا المثيل أسبق أو مساوي أو لاحق للقيمة المحددة من DateTime.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | كائن DateTime معبأ للمقارنة، أو null. |

**Returns:**
int - رقم موقع يشير إلى القيم النسبية لهذه المثيلة والقيمة. الوصف القيمة أقل من الصفر هذه المثيلة أقدم من القيمة. صفر هذه المثيلة هي نفسها القيمة. أكبر من الصفر هذه المثيلة أحدث من القيمة، أو القيمة هي null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


يعيد قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | كائن للمقارنة مع هذه المثيلة. |

**Returns:**
boolean - true إذا كان value مثيلة من DateTime وتساوي قيمة هذه المثيلة؛ وإلا false.
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


يحصل على يوم الشهر الممثل بهذا المثيل.

**Returns:**
int - مكوّن اليوم، يُعبّر عنه كقيمة بين 1 و31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


يحصل على يوم الأسبوع الممثل بهذا المثيل.

**Returns:**
int - يوم الأسبوع لهذه القيمة من DateTime.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


يحصل على يوم السنة الممثل بهذا المثيل.

**Returns:**
int - يوم السنة، يُعبّر عنه كقيمة بين 1 و366.
### getHour() {#getHour--}
```
public int getHour()
```


يحصل على مكوّن الساعة من التاريخ الممثل بهذا المثيل.

**Returns:**
int - مكوّن الساعة، يُعبّر عنه كقيمة بين 0 و23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


يحصل على مكوّن المللي ثانية من التاريخ الممثل بهذا المثيل.

**Returns:**
int - مكوّن الميللي ثانية، يُعبّر عنه كقيمة بين 0 و999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


يحصل على مكوّن الدقيقة من التاريخ الممثل بهذا المثيل.

**Returns:**
int - مكوّن الدقيقة، يُعبّر عنه كقيمة بين 0 و59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


يحصل على مكوّن الشهر من التاريخ الممثل بهذا المثيل.

**Returns:**
int - مكوّن الشهر، يُعبّر عنه كقيمة بين 1 و12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


يحصل على كائن DateTime مضبوط على التاريخ والوقت الحاليين على هذا الحاسوب، معبرًا عنهما بالتوقيت المحلي.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


يحصل على مكوّن الثواني من التاريخ الممثل بهذا المثيل.

**Returns:**
int - الثواني، بين 0 و59.
### getYear() {#getYear--}
```
public int getYear()
```


يحصل على مكوّن السنة من التاريخ الممثل بهذا المثيل.

**Returns:**
int - السنة، بين 1 و9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد رمز التجزئة لهذا المثيل.

**Returns:**
int - رمز تجزئة موقع 32-بت.
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


يحوِّل قيمة كائن DateTime الحالي إلى كائن Calendar.

**Returns:**
java.util.Calendar - كائن Calendar
### toDate() {#toDate--}
```
public Date toDate()
```


يحوِّل قيمة كائن DateTime الحالي إلى كائن Date.

**Returns:**
java.util.Date - كائن Date
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


يحوِّل قيمة كائن DateTime الحالي إلى الوقت المحلي.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


يحوِّل قيمة كائن DateTime الحالي إلى تمثيله النصي المكافئ.

**Returns:**
java.lang.String - تمثيل نصي لقيمة كائن DateTime الحالي.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


يحوِّل قيمة كائن DateTime الحالي إلى الوقت العالمي المنسق (UTC).

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of UTC
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

