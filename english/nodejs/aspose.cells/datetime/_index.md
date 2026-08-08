---
title: "DateTime"
linktitle: "DateTime"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents an instant in time, typically expressed as a date and time of day."
type: docs
weight: 1070
url: /nodejs/aspose.cells/datetime/
---

## DateTime class

Represents an instant in time, typically expressed as a date and time of day.

```js
new DateTime(year, month, day)
```

Initializes a new instance of the DateTime object to the specified year, month, and day.

## Methods

| Name | Description |
| --- | --- |
| [addDays(value)](#adddays) | Adds the specified number of days to the value of this instance. |
| [addHours(value)](#addhours) | Adds the specified number of hours to the value of this instance. |
| [addMilliseconds(value)](#addmilliseconds) | Adds the specified number of milliseconds to the value of this instance. |
| [addMinutes(value)](#addminutes) | Adds the specified number of minutes to the value of this instance. |
| [addMonths(months)](#addmonths) | Adds the specified number of months to the value of this instance. |
| [addSeconds(value)](#addseconds) | Adds the specified number of seconds to the value of this instance. |
| [addYears(value)](#addyears) | Adds the specified number of years to the value of this instance. |
| [compareTo(value)](#compareto) | Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integ |
| [compareTo(value)](#compareto-1) | Compares the value of this instance to a specified DateTime value and returns an integer that indicates whether this ins |
| [constructor_overload$1(year, month, day, hour, minute, second)](#constructor-overload1) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second. |
| [constructor_overload$2(year, month, day, hour, minute, second, millisecond)](#constructor-overload2) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and milliseco |
| [constructor_overload$3(date)](#constructor-overload3) | Initializes a new instance of the DateTime object to the specified Date object |
| [constructor_overload$4(cld)](#constructor-overload4) | Initializes a new instance of the DateTime object to the specified Calendar object |
| [equals(value)](#equals) | Returns a value indicating whether this instance is equal to a specified object. |
| [getDay()](#getday) | Gets the day of the month represented by this instance. |
| [getDayOfWeek()](#getdayofweek) | Gets the day of the week represented by this instance. |
| [getDayOfYear()](#getdayofyear) | Gets the day of the year represented by this instance. |
| [getHour()](#gethour) | Gets the hour component of the date represented by this instance. |
| [getMillisecond()](#getmillisecond) | Gets the milliseconds component of the date represented by this instance. |
| [getMinute()](#getminute) | Gets the minute component of the date represented by this instance. |
| [getMonth()](#getmonth) | Gets the month component of the date represented by this instance. |
| [getSecond()](#getsecond) | Gets the seconds component of the date represented by this instance. |
| [getYear()](#getyear) | Gets the year component of the date represented by this instance. |
| [hashCode()](#hashcode) | Returns the hash code for this instance. |
| [toCalendar()](#tocalendar) | Converts the value of the current DateTime object to Calendar object. |
| [toDate()](#todate) | Converts the value of the current DateTime object to Date object. |
| [toLocalTime()](#tolocaltime) | Converts the value of the current DateTime object to local time. |
| [toString()](#tostring) | Converts the value of the current DateTime object to its equivalent string representation. |
| [toUniversalTime()](#touniversaltime) | Converts the value of the current DateTime object to Coordinated Universal Time(UTC). |
| [getNow()](#getnow) *(static)* | Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time. |

### addDays(value) {#adddays}

Adds the specified number of days to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of whole and fractional days. The value parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.

### addHours(value) {#addhours}

Adds the specified number of hours to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of whole and fractional hours. The value parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.

### addMilliseconds(value) {#addmilliseconds}

Adds the specified number of milliseconds to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of whole and fractional milliseconds. The value parameter can be negative or positive. Note that this value is rounded to the nearest integer. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.

### addMinutes(value) {#addminutes}

Adds the specified number of minutes to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of whole and fractional minutes. The value parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.

### addMonths(months) {#addmonths}

Adds the specified number of months to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| months | Number | A number of months. The months parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and months.

### addSeconds(value) {#addseconds}

Adds the specified number of seconds to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of whole and fractional seconds. The value parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.

### addYears(value) {#addyears}

Adds the specified number of years to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Number | A number of years. The value parameter can be negative or positive. |

**Returns:** DateTime — `DateTime` A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.

### compareTo(value) {#compareto}

Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | A boxed DateTime object to compare, or null. |

**Returns:** Number — `Number` A signed number indicating the relative values of this instance and value. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value, or value is null.

### compareTo(value) {#compareto-1}

Compares the value of this instance to a specified DateTime value and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.

| Parameter | Type | Description |
| --- | --- | --- |
| value | DateTime | A DateTime object to compare. |

**Returns:** Number — `Number` A signed number indicating the relative values of this instance and the value parameter. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value.

### constructor_overload$1(year, month, day, hour, minute, second) {#constructor-overload1}

Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second.

| Parameter | Type | Description |
| --- | --- | --- |
| year | Number | The year (1 through 9999). |
| month | Number | The month (1 through 12). |
| day | Number | The day (1 through the number of days in month). |
| hour | Number | The hours (0 through 23). |
| minute | Number | The minutes (0 through 59). |
| second | Number | The seconds (0 through 59). |

### constructor_overload$2(year, month, day, hour, minute, second, millisecond) {#constructor-overload2}

Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and millisecond.

| Parameter | Type | Description |
| --- | --- | --- |
| year | Number | The year (1 through 9999). |
| month | Number | The month (1 through 12). |
| day | Number | The day (1 through the number of days in month). |
| hour | Number | The hours (0 through 23). |
| minute | Number | The minutes (0 through 59). |
| second | Number | The seconds (0 through 59). |
| millisecond | Number | The milliseconds (0 through 999). |

### constructor_overload$3(date) {#constructor-overload3}

Initializes a new instance of the DateTime object to the specified Date object

| Parameter | Type | Description |
| --- | --- | --- |
| date | Date | The Date object |

### constructor_overload$4(cld) {#constructor-overload4}

Initializes a new instance of the DateTime object to the specified Calendar object

| Parameter | Type | Description |
| --- | --- | --- |
| cld | Calendar | The Calendar object |

### equals(value) {#equals}

Returns a value indicating whether this instance is equal to a specified object.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | An object to compare to this instance. |

**Returns:** boolean — `boolean` true if value is an instance of DateTime and equals the value of this instance; otherwise, false.

### getDay() {#getday}

Gets the day of the month represented by this instance.

**Returns:** Number — `Number` The day component, expressed as a value between 1 and 31.

### getDayOfWeek() {#getdayofweek}

Gets the day of the week represented by this instance.

**Returns:** Number — `Number` the day of the week of this DateTime value.

### getDayOfYear() {#getdayofyear}

Gets the day of the year represented by this instance.

**Returns:** Number — `Number` The day of the year, expressed as a value between 1 and 366.

### getHour() {#gethour}

Gets the hour component of the date represented by this instance.

**Returns:** Number — `Number` The hour component, expressed as a value between 0 and 23.

### getMillisecond() {#getmillisecond}

Gets the milliseconds component of the date represented by this instance.

**Returns:** Number — `Number` The milliseconds component, expressed as a value between 0 and 999.

### getMinute() {#getminute}

Gets the minute component of the date represented by this instance.

**Returns:** Number — `Number` The minute component, expressed as a value between 0 and 59.

### getMonth() {#getmonth}

Gets the month component of the date represented by this instance.

**Returns:** Number — `Number` The month component, expressed as a value between 1 and 12.

### getSecond() {#getsecond}

Gets the seconds component of the date represented by this instance.

**Returns:** Number — `Number` The seconds, between 0 and 59.

### getYear() {#getyear}

Gets the year component of the date represented by this instance.

**Returns:** Number — `Number` The year, between 1 and 9999.

### hashCode() {#hashcode}

Returns the hash code for this instance.

**Returns:** Number — `Number` A 32-bit signed integer hash code.

### toCalendar() {#tocalendar}

Converts the value of the current DateTime object to Calendar object.

**Returns:** Calendar — `Calendar` Calendar object

### toDate() {#todate}

Converts the value of the current DateTime object to Date object.

**Returns:** Date — `Date` Date object

### toLocalTime() {#tolocaltime}

Converts the value of the current DateTime object to local time.

**Returns:** DateTime — `DateTime` A DateTime object of local

### toString() {#tostring}

Converts the value of the current DateTime object to its equivalent string representation.

**Returns:** String — `String` A string representation of the value of the current DateTime object.

### toUniversalTime() {#touniversaltime}

Converts the value of the current DateTime object to Coordinated Universal Time(UTC).

**Returns:** DateTime — `DateTime` A DateTime object of UTC

### getNow() (static) {#getnow}

Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time.

**Returns:** DateTime — `DateTime` A DateTime object whose value is the current local date and time.
