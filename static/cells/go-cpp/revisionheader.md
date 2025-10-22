##RevisionHeader Class
'RevisionHeader class. Encapsulates the object that represents revisionheader in Go.'
## RevisionHeader class
Represents a list of specific changes that have taken place for this workbook.
```go
type RevisionHeader struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionHeader](./newrevisionheader/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSavedTime](./getsavedtime/) | Gets and sets rhe date and time when this set of revisions was saved. |
|[SetSavedTime](./setsavedtime/) | Gets and sets rhe date and time when this set of revisions was saved. |
|[Get_UserName](./get_username/) | Gets and sets the name of the user making the revision. |
|[SetUserName](./setusername/) | Gets and sets the name of the user making the revision. |
