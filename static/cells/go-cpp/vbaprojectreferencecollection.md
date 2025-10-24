##VbaProjectReferenceCollection Class
'VbaProjectReferenceCollection class. Encapsulates the object that represents vbaprojectreferencecollection in Go.'
## VbaProjectReferenceCollection class
Represents all references of VBA project.
```go
type VbaProjectReferenceCollection struct  {
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
|[Get](./get/) | Get the reference in the list by the index. |
|[AddRegisteredReference](./addregisteredreference/) | Add a reference to an Automation type library. |
|[AddControlRefrernce](./addcontrolrefrernce/) | Add a reference to a twiddled type library and its extended type library. |
|[AddProjectRefrernce](./addprojectrefrernce/) | Adds a reference to an external VBA project. |
|[Copy](./copy/) | Copies references from other VBA project. |
|[GetCount](./getcount/) |  |
