##DataModelRelationship Class
'DataModelRelationship class. Encapsulates the object that represents datamodelrelationship in Go.'
## DataModelRelationship class
Represents a single relationship in the spreadsheet data model.
```go
type DataModelRelationship struct  {
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
|[GetForeignKeyTable](./getforeignkeytable/) | Gets the name of the foreign key table for this relationship. |
|[GetPrimaryKeyTable](./getprimarykeytable/) | Gets the name of the primary key table for this relationship. |
|[GetForeignKeyColumn](./getforeignkeycolumn/) | Gets the name of the foreign key table column for this relationship. |
|[GetPrimaryKeyColumn](./getprimarykeycolumn/) | Gets the name of the primary key table column for this relationship. |
