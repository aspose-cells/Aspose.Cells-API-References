##WriteProtection Class
'WriteProtection class. Encapsulates the object that represents writeprotection in Go.'
## WriteProtection class
Specifies write protection settings for a workbook.
```go
type WriteProtection struct  {
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
|[GetAuthor](./getauthor/) | Gets and sets the author. |
|[SetAuthor](./setauthor/) | Gets and sets the author. |
|[GetRecommendReadOnly](./getrecommendreadonly/) | Indicates if the Read Only Recommended option is selected. |
|[SetRecommendReadOnly](./setrecommendreadonly/) | Indicates if the Read Only Recommended option is selected. |
|[IsWriteProtected](./iswriteprotected/) | Indicates whether this workbook is write protected. |
|[GetPassword](./getpassword/) | Sets the protected password to modify the file. |
|[SetPassword](./setpassword/) | Sets the protected password to modify the file. |
|[ValidatePassword](./validatepassword/) | Returns true if the specified password is the same as the write-protection password the file was protected with. |
