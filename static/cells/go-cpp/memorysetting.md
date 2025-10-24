##MemorySetting Enum
'MemorySetting enum. Encapsulates the object that represents memorysetting in Go.'
## MemorySetting Enum
Memory usage modes for cells data model.
```go
type MemorySetting int32
```
## Fields
| Field | Description |
| --- | --- |
|[Normal](./normal/) | Default mode for cells model. |
|[MemoryPreference](./memorypreference/) | Memory performance preferable. |
|[FileCache](./filecache/) | Memory performance preferable and using file instead of memoryto maintain the cells data. |
