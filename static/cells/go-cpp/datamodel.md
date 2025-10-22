##DataModel Class
'DataModel class. Encapsulates the object that represents datamodel in Go.'
## DataModel class
Represents the data model.
```go
type DataModel struct  {
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
|[GetRelationships](./getrelationships/) | Gets all relationships of the tables in the data model. |
|[GetTables](./gettables/) | Gets all tables in the data model. |
