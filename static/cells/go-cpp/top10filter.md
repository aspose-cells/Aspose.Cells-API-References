##Top10Filter Class
'Top10Filter class. Encapsulates the object that represents top10filter in Go.'
## Top10Filter class
Represents the top 10 filter.
```go
type Top10Filter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTop10Filter](./newtop10filter/) | Constructs from an Object convertible to this. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[ToObject](./toobject/) | Gets the Object. |
|[IsTop](./istop/) | Indicates whether it's top filter. |
|[SetIsTop](./setistop/) | Indicates whether it's top filter. |
|[IsPercent](./ispercent/) | Indicates whether the items is percent. |
|[SetIsPercent](./setispercent/) | Indicates whether the items is percent. |
|[GetItems](./getitems/) | Gets and sets the items of the filter. |
|[SetItems](./setitems/) | Gets and sets the items of the filter. |
|[GetCriteria](./getcriteria/) |  |
|[SetCriteria](./setcriteria/) |  |
