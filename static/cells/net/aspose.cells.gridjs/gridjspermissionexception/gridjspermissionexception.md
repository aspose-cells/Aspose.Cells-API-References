##GridJsPermissionException.GridJsPermissionException
GridJsPermissionException constructor. Constructs a permission exception
## GridJsPermissionException(string, CoWorkUserPermission, CoWorkUserPermission) {#constructor}
Constructs a permission exception
```csharp
public GridJsPermissionException(string operation, CoWorkUserPermission requiredPermission,
CoWorkUserPermission currentPermission)
```
| Parameter | Type | Description |
| --- | --- | --- |
| operation | String | Operation attempted to execute |
| requiredPermission | CoWorkUserPermission | Permission required for the operation |
| currentPermission | CoWorkUserPermission | Current user permission |
### See Also
* enum [CoWorkUserPermission](../../coworkuserpermission/)
* class [GridJsPermissionException](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
## GridJsPermissionException(string, string, CoWorkUserPermission, CoWorkUserPermission) {#constructor_1}
Constructs a permission exception
```csharp
public GridJsPermissionException(string message, string operation,
CoWorkUserPermission requiredPermission, CoWorkUserPermission currentPermission)
```
| Parameter | Type | Description |
| --- | --- | --- |
| message | String | Custom error message |
| operation | String | Operation attempted to execute |
| requiredPermission | CoWorkUserPermission | Permission required for the operation |
| currentPermission | CoWorkUserPermission | Current user permission |
### See Also
* enum [CoWorkUserPermission](../../coworkuserpermission/)
* class [GridJsPermissionException](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
