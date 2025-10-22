##ErrorCheckOption Class
'ErrorCheckOption class. Encapsulates the object that represents errorcheckoption in Go.'
## ErrorCheckOption class
Error check setting applied on certain ranges.
```go
type ErrorCheckOption struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsErrorCheck](./iserrorcheck/) | Checks whether given error type will be checked. |
|[SetErrorCheck](./seterrorcheck/) | Sets whether given error type will be checked. |
|[GetCountOfRange](./getcountofrange/) | Gets the count of ranges that influenced by this setting. |
|[AddRange](./addrange/) | Adds one influenced range by this setting. |
|[GetRange](./getrange/) | Gets the influenced range of this setting by given index. |
|[RemoveRange](./removerange/) | Removes one range by given index. |
