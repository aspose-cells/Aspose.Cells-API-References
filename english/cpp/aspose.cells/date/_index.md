---
title: Aspose::Cells::Date struct
linktitle: Date
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Date struct. Represents a date and time in C++.'
type: docs
weight: 28800
url: /cpp/aspose.cells/date/
---
## Date struct


Represents a date and time.

```cpp
struct Date
```

## Methods

| Method | Description |
| --- | --- |
| [AddDays(double days)](./adddays/) const | Returns a new [Date](./) that adds the specified number of days. |
| [AddHours(double hours)](./addhours/) const | Returns a new [Date](./) that adds the specified number of hours. |
| [AddMilliseconds(double ms)](./addmilliseconds/) const | Returns a new [Date](./) that adds the specified number of milliseconds. |
| [AddMinutes(double minutes)](./addminutes/) const | Returns a new [Date](./) that adds the specified number of minutes. |
| [AddMonths(int32_t months)](./addmonths/) const | Returns a new [Date](./) that adds the specified number of months. |
| [AddSeconds(double seconds)](./addseconds/) const | Returns a new [Date](./) that adds the specified number of seconds. |
| [AddYears(int32_t years)](./addyears/) const | Returns a new [Date](./) that adds the specified number of years. |
| [DayOfWeek()](./dayofweek/) const | Gets the day of the week for this date. |
| static [FromEpochMillisecondsUTC(int64_t ms)](./fromepochmillisecondsutc/) | Creates a [Date](./) from Unix epoch milliseconds (UTC). |
| static [Now()](./now/) | Gets the current local date and time. |
| static [NowUTC()](./nowutc/) | Gets the current UTC date and time. |
| [operator!=(const Date\& other)](./operator!_asm/) const | Determines whether two [Date](./) instances represent different points in time. |
| [operator+(const Duration\& ts)](./operator+/) const | Adds a time interval to the current [Date](./). |
| [operator-(const Duration\& ts)](./operator-/) const | Subtracts a time interval from the current [Date](./). |
| [operator-(const Date\& other)](./operator-/) const | Computes the difference between two [Date](./) instances. |
| [operator<(const Date\& other)](./operator_lt/) const | Determines whether this instance is earlier than another [Date](./). |
| [operator<=(const Date\& other)](./operator_lt_asm/) const | Determines whether this instance is earlier than or equal to another [Date](./). |
| [operator==(const Date\& other)](./operator_asm_asm/) const | Determines whether two [Date](./) instances represent the same point in time. |
| [operator>(const Date\& other)](./operator_gt/) const | Determines whether this instance is later than another [Date](./). |
| [operator>=(const Date\& other)](./operator_gt_asm/) const | Determines whether this instance is later than or equal to another [Date](./). |
| static [Parse(const U16String\& str)](./parse/) | Parses a string into a [Date](./) using default format rules. |
| static [Parse(const U16String\& str, const U16String\& format)](./parse/) | Parses a string into a [Date](./) using a specified format. |
| [ToEpochMillisecondsUTC()](./toepochmillisecondsutc/) const | Converts this [Date](./) to Unix epoch time in milliseconds (UTC). |
| [ToLocal()](./tolocal/) const | Converts this [Date](./) to local system time. |
| [ToString()](./tostring/) const | Converts this [Date](./) to its default string representation. |
| [ToString(const U16String\& format)](./tostring/) const | Converts this [Date](./) to a string using the specified format. |
| [ToUTC()](./toutc/) const | Converts this [Date](./) to Coordinated Universal Time (UTC). |
## Fields

| Field | Description |
| --- | --- |
| [dateKind](./datekind/) | Specifies whether the time is local, UTC, or unspecified. Default value is Unspecified. |
| [day](./day/) | Day component (1-31). |
| [hour](./hour/) | Hour component (0-23). |
| [millisecond](./millisecond/) | Millisecond component (0-999). |
| [minute](./minute/) | Minute component (0-59). |
| [month](./month/) | Month component (1-12). |
| [second](./second/) | Second component (0-59). |
| [year](./year/) | Year component (1-9999). |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
