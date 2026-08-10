---
title: "DateTime Class"
linktitle: "DateTime"
articleTitle: "DateTime"
second_title: "Aspose.Cells for Python via Java"
description: "Represents an instant in time, typically expressed as a date and time of day."
type: docs
weight: 1640
url: /python-java/asposecells.api/datetime/
---

## DateTime class

Represents an instant in time, typically expressed as a date and time of day.

## Constructors

| Name | Description |
| --- | --- |
| [DateTime](#constructor) | Initializes a new instance of the DateTime object to the specified year, month, and day. |
| [DateTime](#constructor) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second. |
| [DateTime](#constructor) | Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and milliseco |
| [DateTime](#constructor) | Initializes a new instance of the DateTime object to the specified Date object |
| [DateTime](#constructor) | Initializes a new instance of the DateTime object to the specified Calendar object |

## Methods

| Name | Description |
| --- | --- |
| [toDate](#todate) | Converts the value of the current DateTime object to Date object. |
| [toCalendar](#tocalendar) | Converts the value of the current DateTime object to Calendar object. |
| [toUniversalTime](#touniversaltime) | Converts the value of the current DateTime object to Coordinated Universal Time(UTC). |
| [toLocalTime](#tolocaltime) | Converts the value of the current DateTime object to local time. |
| [addDays](#adddays) | Adds the specified number of days to the value of this instance. |
| [addHours](#addhours) | Adds the specified number of hours to the value of this instance. |
| [addMilliseconds](#addmilliseconds) | Adds the specified number of milliseconds to the value of this instance. |
| [addMinutes](#addminutes) | Adds the specified number of minutes to the value of this instance. |
| [addMonths](#addmonths) | Adds the specified number of months to the value of this instance. |
| [addSeconds](#addseconds) | Adds the specified number of seconds to the value of this instance. |
| [addYears](#addyears) | Adds the specified number of years to the value of this instance. |
| [compareTo](#compareto) | Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integ |
| [hashCode](#hashcode) | Returns the hash code for this instance. |
| [equals](#equals) | Returns a value indicating whether this instance is equal to a specified object. |
| [getDay](#getday) | Gets the day of the month represented by this instance. |
| [getDayOfWeek](#getdayofweek) | Gets the day of the week represented by this instance. |
| [getDayOfYear](#getdayofyear) | Gets the day of the year represented by this instance. |
| [getHour](#gethour) | Gets the hour component of the date represented by this instance. |
| [getMillisecond](#getmillisecond) | Gets the milliseconds component of the date represented by this instance. |
| [getMinute](#getminute) | Gets the minute component of the date represented by this instance. |
| [getMonth](#getmonth) | Gets the month component of the date represented by this instance. |
| [getNow](#getnow) | Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time. |
| [getSecond](#getsecond) | Gets the seconds component of the date represented by this instance. |
| [getYear](#getyear) | Gets the year component of the date represented by this instance. |
| [toString](#tostring) | Converts the value of the current DateTime object to its equivalent string representation. |

### DateTime(year, month, day) (1 of 5) {#constructor}

Initializes a new instance of the DateTime object to the specified year, month, and day.

| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |

---

### DateTime(year, month, day, hour, minute, second) (2 of 5) {#constructor-1}

Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, and second.

| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |
| hour | int | The hours (0 through 23). |
| minute | int | The minutes (0 through 59). |
| second | int | The seconds (0 through 59). |

---

### DateTime(year, month, day, hour, minute, second, millisecond) (3 of 5) {#constructor-2}

Initializes a new instance of the DateTime object to the specified year, month, day, hour, minute, second, and millisecond.

| Parameter | Type | Description |
| --- | --- | --- |
| year | int | The year (1 through 9999). |
| month | int | The month (1 through 12). |
| day | int | The day (1 through the number of days in month). |
| hour | int | The hours (0 through 23). |
| minute | int | The minutes (0 through 59). |
| second | int | The seconds (0 through 59). |
| millisecond | int | The milliseconds (0 through 999). |

---

### DateTime(date) (4 of 5) {#constructor-3}

Initializes a new instance of the DateTime object to the specified Date object

| Parameter | Type | Description |
| --- | --- | --- |
| date | Date | The Date object |

---

### DateTime(cld) (5 of 5) {#constructor-4}

Initializes a new instance of the DateTime object to the specified Calendar object

| Parameter | Type | Description |
| --- | --- | --- |
| cld | Calendar | The Calendar object |

### toDate() {#todate}

Converts the value of the current DateTime object to Date object.

**Returns:** Date object

### toCalendar() {#tocalendar}

Converts the value of the current DateTime object to Calendar object.

**Returns:** Calendar object

### toUniversalTime() {#touniversaltime}

Converts the value of the current DateTime object to Coordinated Universal Time(UTC).

**Returns:** A DateTime object of UTC

### toLocalTime() {#tolocaltime}

Converts the value of the current DateTime object to local time.

**Returns:** A DateTime object of local

### addDays(value) {#adddays}

Adds the specified number of days to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | float | A number of whole and fractional days. The value parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.

### addHours(value) {#addhours}

Adds the specified number of hours to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | float | A number of whole and fractional hours. The value parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.

### addMilliseconds(value) {#addmilliseconds}

Adds the specified number of milliseconds to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | float | A number of whole and fractional milliseconds. The value parameter can be negative or positive. Note that this value is rounded to the nearest integer. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.

### addMinutes(value) {#addminutes}

Adds the specified number of minutes to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | float | A number of whole and fractional minutes. The value parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.

### addMonths(months) {#addmonths}

Adds the specified number of months to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| months | int | A number of months. The months parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and months.

### addSeconds(value) {#addseconds}

Adds the specified number of seconds to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | float | A number of whole and fractional seconds. The value parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.

### addYears(value) {#addyears}

Adds the specified number of years to the value of this instance.

| Parameter | Type | Description |
| --- | --- | --- |
| value | int | A number of years. The value parameter can be negative or positive. |

**Returns:** A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.

### compareTo(value) (1 of 2) {#compareto}

Compares the value of this instance to a specified object that contains a specified DateTime value, and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | A boxed DateTime object to compare, or null. |

**Returns:** A signed number indicating the relative values of this instance and value. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value, or value is null.

---

### compareTo(value) (2 of 2) {#compareto-1}

Compares the value of this instance to a specified DateTime value and returns an integer that indicates whether this instance is earlier than, the same as, or later than the specified DateTime value.

| Parameter | Type | Description |
| --- | --- | --- |
| value | DateTime | A DateTime object to compare. |

**Returns:** A signed number indicating the relative values of this instance and the value parameter. Value Description Less than zero This instance is earlier than value. Zero This instance is the same as value. Greater than zero This instance is later than value.

### hashCode() {#hashcode}

Returns the hash code for this instance.

**Returns:** A 32-bit signed integer hash code.

### equals(value) {#equals}

Returns a value indicating whether this instance is equal to a specified object.

| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | An object to compare to this instance. |

**Returns:** true if value is an instance of DateTime and equals the value of this instance; otherwise, false.

### getDay() {#getday}

Gets the day of the month represented by this instance.

**Returns:** The day component, expressed as a value between 1 and 31.

### getDayOfWeek() {#getdayofweek}

Gets the day of the week represented by this instance.

**Returns:** the day of the week of this DateTime value.

### getDayOfYear() {#getdayofyear}

Gets the day of the year represented by this instance.

**Returns:** The day of the year, expressed as a value between 1 and 366.

### getHour() {#gethour}

Gets the hour component of the date represented by this instance.

**Returns:** The hour component, expressed as a value between 0 and 23.

### getMillisecond() {#getmillisecond}

Gets the milliseconds component of the date represented by this instance.

**Returns:** The milliseconds component, expressed as a value between 0 and 999.

### getMinute() {#getminute}

Gets the minute component of the date represented by this instance.

**Returns:** The minute component, expressed as a value between 0 and 59.

### getMonth() {#getmonth}

Gets the month component of the date represented by this instance.

**Returns:** The month component, expressed as a value between 1 and 12.

### getNow() {#getnow}

Gets a DateTime object that is set to the current date and time on this computer, expressed as the local time.

**Returns:** A DateTime object whose value is the current local date and time.

### getSecond() {#getsecond}

Gets the seconds component of the date represented by this instance.

**Returns:** The seconds, between 0 and 59.

### getYear() {#getyear}

Gets the year component of the date represented by this instance.

**Returns:** The year, between 1 and 9999.

### toString() {#tostring}

Converts the value of the current DateTime object to its equivalent string representation.

**Returns:** A string representation of the value of the current DateTime object.
