##PrintingPageType Enum
'PrintingPageType enum. Encapsulates the object that represents printingpagetype in Go.'
## PrintingPageType Enum
Indicates which pages will not be printed.
```go
type PrintingPageType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Prints all pages. |
|[IgnoreBlank](./ignoreblank/) | Don't print the pages which the cells are blank. |
|[IgnoreStyle](./ignorestyle/) | Don't print the pages which cells only contain styles. |
