##DateTime
Represents an instant in time typically expressed as a date and time of day.
**Inheritance:**
java.lang.Object
```
public class DateTime
```
Represents an instant in time, typically expressed as a date and time of day.
## Constructors
| Constructor | Description |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Initializes a new instance of the DateTime object to the specified year, month, and day. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and millisecond. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Initializes a new instance of the DateTime object to the specified Date object |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Initializes a new instance of the DateTime object to the specified Calendar object |
## Methods
| Method | Description |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Adds the specified number of days to the value of this instance. |
| [addHours(double value)](#addHours-double-) | Adds the specified number of hours to the value of this instance. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Adds the specified number of milliseconds to the value of this instance. |
| [addMinutes(double value)](#addMinutes-double-) | Adds the specified number of minutes to the value of this instance. |
| [addMonths(int months)](#addMonths-int-) | Adds the specified number of months to the value of this instance. |
| [addSeconds(double value)](#addSeconds-double-) | Adds the specified number of seconds to the value of this instance. |
| [addYears(int value)](#addYears-int-) | Adds the specified number of years to the value of this instance. |
| [compareTo(DateTime value)](#compareTo-com.aspose.cells.DateTime-) | Compares the value of this instance to a specified DateTime value and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value. |
| [equals(Object value)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Gets the day of the month represented by this instance. |
| [getDayOfWeek()](#getDayOfWeek--) | Gets the day of the week represented by this instance. |
| [getDayOfYear()](#getDayOfYear--) | Gets the day of the year represented by this instance. |
| [getHour()](#getHour--) | Gets the hour component of the date represented by this instance. |
| [getMillisecond()](#getMillisecond--) | Gets the milliseconds component of the date represented by this instance. |
| [getMinute()](#getMinute--) | Gets the minute component of the date represented by this instance. |
| [getMonth()](#getMonth--) | Gets the month component of the date represented by this instance. |
| [getNow()](#getNow--) | Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time. |
| [getSecond()](#getSecond--) | Gets the seconds component of the date represented by this instance. |
| [getYear()](#getYear--) | Gets the year component of the date represented by this instance. |
| [hashCode()](#hashCode--) | Returns the hash code for this instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Converts the value of the current DateTime object to Calendar object. |
| [toDate()](#toDate--) | Converts the value of the current DateTime object to Date object. |
| [toLocalTime()](#toLocalTime--) | Converts the value of the current DateTime object to local time. |
| [toString()](#toString--) | Converts the value of the current DateTime object to its equivalent string representation. |
| [toUniversalTime()](#toUniversalTime--) | Converts the value of the current DateTime object to Coordinated Universal Time(UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```
Initializes a new instance of the DateTime object to the specified year, month, and day.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |
### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```
Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |
| hour | int | The hours (0 through 23). |
| minute | int | The minutes (0 through 59). |
| second | int | The seconds (0 through 59). |
### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```
Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and millisecond.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |
| hour | int | The hours (0 through 23). |
| minute | int | The minutes (0 through 59). |
| second | int | The seconds (0 through 59). |
| millisecond | int | The milliseconds (0 through 999). |
### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```
Initializes a new instance of the DateTime object to the specified Date object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The Date object |
### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```
Initializes a new instance of the DateTime object to the specified Calendar object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cld | java.util.Calendar | The Calendar object |
### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```
Adds the specified number of days to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | A number of whole and fractional days. The value parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```
Adds the specified number of hours to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | A number of whole and fractional hours. The value parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```
Adds the specified number of milliseconds to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | A number of whole and fractional milliseconds. The value parameter can be negative or positive. Note that this value is rounded to the nearest integer. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```
Adds the specified number of minutes to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | A number of whole and fractional minutes. The value parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```
Adds the specified number of months to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| months | int | A number of months. The months parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```
Adds the specified number of seconds to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | A number of whole and fractional seconds. The value parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```
Adds the specified number of years to the value of this instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | A number of years. The value parameter can be negative or positive. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.cells.DateTime-}
```
public int compareTo(DateTime value)
```
Compares the value of this instance to a specified DateTime value and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) | A DateTime object to compare. |
**Returns:**
int - A signed number indicating the relative values of this instance and the value parameter. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```
Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | A boxed DateTime object to compare, or null. |
**Returns:**
int - A signed number indicating the relative values of this instance and value. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value, or value is null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```
Returns a value indicating whether this instance is equal to a specified object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | An object to compare to this instance. |
**Returns:**
boolean - true if value is an instance of DateTime and equals the value of this instance; otherwise, false.
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
Gets the day of the month represented by this instance.
**Returns:**
int - The day component, expressed as a value between 1 and 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```
Gets the day of the week represented by this instance.
**Returns:**
int - the day of the week of this DateTime value.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```
Gets the day of the year represented by this instance.
**Returns:**
int - The day of the year, expressed as a value between 1 and 366.
### getHour() {#getHour--}
```
public int getHour()
```
Gets the hour component of the date represented by this instance.
**Returns:**
int - The hour component, expressed as a value between 0 and 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```
Gets the milliseconds component of the date represented by this instance.
**Returns:**
int - The milliseconds component, expressed as a value between 0 and 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```
Gets the minute component of the date represented by this instance.
**Returns:**
int - The minute component, expressed as a value between 0 and 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```
Gets the month component of the date represented by this instance.
**Returns:**
int - The month component, expressed as a value between 1 and 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```
Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time.
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```
Gets the seconds component of the date represented by this instance.
**Returns:**
int - The seconds, between 0 and 59.
### getYear() {#getYear--}
```
public int getYear()
```
Gets the year component of the date represented by this instance.
**Returns:**
int - The year, between 1 and 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```
Returns the hash code for this instance.
**Returns:**
int - A 32-bit signed integer hash code.
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
Converts the value of the current DateTime object to Calendar object.
**Returns:**
java.util.Calendar - Calendar object
### toDate() {#toDate--}
```
public Date toDate()
```
Converts the value of the current DateTime object to Date object.
**Returns:**
java.util.Date - Date object
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```
Converts the value of the current DateTime object to local time.
**Returns:**
[DateTime](../../com.aspose.cells/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```
Converts the value of the current DateTime object to its equivalent string representation.
**Returns:**
java.lang.String - A string representation of the value of the current DateTime object.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```
Converts the value of the current DateTime object to Coordinated Universal Time(UTC).
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
