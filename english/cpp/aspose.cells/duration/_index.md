---
title: Aspose::Cells::Duration struct
linktitle: Duration
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Duration struct. Represents a time interval with a resolution of 100 nanoseconds (tick) in C++.'
type: docs
weight: 28900
url: /cpp/aspose.cells/duration/
---
## Duration struct


Represents a time interval with a resolution of 100 nanoseconds (tick).

```cpp
struct Duration
```

## Methods

| Method | Description |
| --- | --- |
| [Duration(int64_t v)](./duration/) | Initializes a new instance from a tick value. |
| [Duration(int hours, int minutes, int seconds)](./duration/) | Initializes a new instance from hours, minutes, and seconds. |
| [Duration(int days, int hours, int minutes, int seconds)](./duration/) | Initializes a new instance from days, hours, minutes, and seconds. |
| [Duration(int days, int hours, int minutes, int seconds, int milliseconds)](./duration/) | Initializes a new instance from days, hours, minutes, seconds, and milliseconds. |
| static [FromDays(double value)](./fromdays/) | Creates a [Duration](./) from a specified number of days. |
| static [FromMilliseconds(double value)](./frommilliseconds/) | Creates a [Duration](./) from a specified number of milliseconds. |
| static [FromMinutes(double value)](./fromminutes/) | Creates a [Duration](./) from a specified number of minutes. |
| static [FromSeconds(double value)](./fromseconds/) | Creates a [Duration](./) from a specified number of seconds. |
| static [FromTicks(int64_t value)](./fromticks/) | Creates a [Duration](./) from a specified number of ticks. |
| [GetDays()](./getdays/) const | Gets the day component of the time interval. |
| [GetHours()](./gethours/) const | Gets the hour component (0-23). |
| [GetMilliseconds()](./getmilliseconds/) const | Gets the millisecond component (0-999). |
| [GetMinutes()](./getminutes/) const | Gets the minute component (0-59). |
| [GetSeconds()](./getseconds/) const | Gets the second component (0-59). |
| [GetTicks()](./getticks/) const | Gets the total number of ticks represented by this instance. |
| [GetTotalDays()](./gettotaldays/) const | Gets the total number of days represented by this instance. |
| [GetTotalHours()](./gettotalhours/) const | Gets the total number of hours represented by this instance. |
| [GetTotalMilliseconds()](./gettotalmilliseconds/) const | Gets the total number of milliseconds represented by this instance. |
| [GetTotalMinutes()](./gettotalminutes/) const | Gets the total number of minutes represented by this instance. |
| [GetTotalSeconds()](./gettotalseconds/) const | Gets the total number of seconds represented by this instance. |
| [operator!=(const Duration\& ts)](./operator!_asm/) const | Determines whether two [Duration](./) instances are not equal. |
| [operator*(double factor)](./operator_lowast/) const | Multiplies the time interval by a scalar factor. |
| [operator+(const Duration\& ts)](./operator+/) const | Adds two time intervals. |
| [operator+()](./operator+/) const | Returns the current instance (unary plus). |
| [operator-(const Duration\& ts)](./operator-/) const | Subtracts one time interval from another. |
| [operator-()](./operator-/) const | Returns a new [Duration](./) whose value is the negation of the current instance. |
| [operator/(const Duration\& ts)](./operator//) const | Returns the ratio between two time intervals. |
| [operator/(double divisor)](./operator//) const | Divides the time interval by a scalar value. |
| [operator<(const Duration\& ts)](./operator_lt/) const | Determines whether the current instance is less than another. |
| [operator<=(const Duration\& ts)](./operator_lt_asm/) const | Determines whether the current instance is less than or equal to another. |
| [operator==(const Duration\& ts)](./operator_asm_asm/) const | Determines whether two [Duration](./) instances are equal. |
| [operator>(const Duration\& ts)](./operator_gt/) const | Determines whether the current instance is greater than another. |
| [operator>=(const Duration\& ts)](./operator_gt_asm/) const | Determines whether the current instance is greater than or equal to another. |
## Fields

| Field | Description |
| --- | --- |
| [value](./value/) | Internal representation of the time interval in ticks. 1 tick = 100 nanoseconds. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
