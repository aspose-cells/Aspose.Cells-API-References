##DisplayUnitType Enum
'DisplayUnitType enum. Encapsulates the object that represents displayunittype in Go.'
## DisplayUnitType Enum
Represents the type of display unit of chart's axis.
```go
type DisplayUnitType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | Display unit is None. |
|[Hundreds](./hundreds/) | Specifies the values on the chart shall be divided by 100. |
|[Thousands](./thousands/) | Specifies the values on the chart shall be divided by 1,000. |
|[TenThousands](./tenthousands/) | Specifies the values on the chart shall be divided by 10,000. |
|[HundredThousands](./hundredthousands/) | Specifies the values on the chart shall be divided by 100,000. |
|[Millions](./millions/) | Specifies the values on the chart shall be divided by 1,000,000. |
|[TenMillions](./tenmillions/) | Specifies the values on the chart shall be divided by 10,000,000. |
|[HundredMillions](./hundredmillions/) | Specifies the values on the chart shall be divided by 100,000,000. |
|[Billions](./billions/) | Specifies the values on the chart shall be divided by 1,000,000,000. |
|[Trillions](./trillions/) | Specifies the values on the chart shall be divided by 1,000,000,000,000. |
|[Percentage](./percentage/) | The values on the chart shall be divided by 0.01. |
|[Cust](./cust/) | specifies a custom value for the display unit. |
|[Custom](./custom/) | specifies a custom value for the display unit. |
