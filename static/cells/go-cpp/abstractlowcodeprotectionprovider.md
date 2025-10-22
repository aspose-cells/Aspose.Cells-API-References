##AbstractLowCodeProtectionProvider Class
'AbstractLowCodeProtectionProvider class. Encapsulates the object that represents abstractlowcodeprotectionprovider in Go.'
## AbstractLowCodeProtectionProvider class
Implementation to provide protection settings
```go
type AbstractLowCodeProtectionProvider struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewAbstractLowCodeProtectionProvider](./newabstractlowcodeprotectionprovider/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOpenPassword](./getopenpassword/) | Gets the password to open spread sheet file. |
|[GetWritePassword](./getwritepassword/) | Gets the password to modify spread sheet file. |
|[GetWorkbookPassword](./getworkbookpassword/) | Gets the password to protect the workbook with specified protection type. |
|[GetWorkbookProtectionType](./getworkbookprotectiontype/) | Gets the protection type to protect the workbook. |
|[GetWorksheetPassword](./getworksheetpassword/) | Gets the password to protect the specified worksheet. |
|[GetWorksheetProtectionType](./getworksheetprotectiontype/) | Gets the protection type to protect the specified worksheet. |
