##TimePeriodType Enum
'TimePeriodType enum. Encapsulates the object that represents timeperiodtype in Go.'
## TimePeriodType Enum
Used in a FormatConditionType.TimePeriod conditional formatting rule.These are dynamic time periods, which change based onthe date the conditional formatting is refreshed / applied.
```go
type TimePeriodType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Today](./today/) | Today's date. |
|[Yesterday](./yesterday/) | Yesterday's date. |
|[Tomorrow](./tomorrow/) | Tomorrow's date. |
|[Last7Days](./last7days/) | A date in the last seven days. |
|[ThisMonth](./thismonth/) | A date occurring in this calendar month. |
|[LastMonth](./lastmonth/) | A date occurring in the last calendar month. |
|[NextMonth](./nextmonth/) | A date occurring in the next calendar month. |
|[ThisWeek](./thisweek/) | A date occurring this week. |
|[LastWeek](./lastweek/) | A date occurring last week. |
|[NextWeek](./nextweek/) | A date occurring next week. |
|[ThisYear](./thisyear/) | A date occurring this year.Only for .ods. |
|[LastYear](./lastyear/) | A date occurring last year.Only for .ods. |
|[NextYear](./nextyear/) | A date occurring next year.Only for .ods. |
