##ProtectedRange Class
'ProtectedRange class. Encapsulates the object that represents protectedrange in Go.'
## ProtectedRange class
A specified range to be allowed to edit when the sheet protection is ON.
```go
type ProtectedRange struct  {
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
|[GetName](./getname/) | Gets the Range title. This is used as a descriptor, not as a named range definition. |
|[SetName](./setname/) | Gets the Range title. This is used as a descriptor, not as a named range definition. |
|[GetCellArea](./getcellarea/) | Gets the CellArea object represents the cell area to be protected. |
|[GetAreas](./getareas/) | Gets all referred areas. |
|[AddArea](./addarea/) | Adds a referred area to this |
|[IsProtectedWithPassword](./isprotectedwithpassword/) | Indicates whether the worksheets is protected with password. |
|[GetPassword](./getpassword/) | Represents the password to protect the range. |
|[SetPassword](./setpassword/) | Represents the password to protect the range. |
|[GetSecurityDescriptor](./getsecuritydescriptor/) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
|[SetSecurityDescriptor](./setsecuritydescriptor/) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
