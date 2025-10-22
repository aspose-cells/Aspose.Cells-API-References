##VbaProject Class
'VbaProject class. Encapsulates the object that represents vbaproject in Go.'
## VbaProject class
Represents the VBA project.
```go
type VbaProject struct  {
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
|[Sign](./sign/) | Sign this VBA project by a DigitalSignature |
|[IsValidSigned](./isvalidsigned/) | Indicates whether the signature of VBA project is valid or not. |
|[GetCertRawData](./getcertrawdata/) | Gets certificate raw data if this VBA project is signed. |
|[GetEncoding](./getencoding/) | Gets and sets the encoding of VBA project. |
|[SetEncoding](./setencoding/) | Gets and sets the encoding of VBA project. |
|[GetName](./getname/) | Gets and sets the name of the VBA project. |
|[SetName](./setname/) | Gets and sets the name of the VBA project. |
|[IsSigned](./issigned/) | Indicates whether VBAcode is signed or not. |
|[Protect](./protect/) | Protects or unprotects this VBA project. |
|[IsProtected](./isprotected/) | Indicates whether this VBA project is protected. |
|[GetIslockedForViewing](./getislockedforviewing/) | Indicates whether this VBA project is locked for viewing. |
|[Copy](./copy/) | Copy VBA project from other file. |
|[GetModules](./getmodules/) | Gets all VbaModule objects. |
|[GetReferences](./getreferences/) | Gets all references of VBA project. |
|[ValidatePassword](./validatepassword/) | Validates protection password. |
