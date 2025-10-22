##Format3D Class
'Format3D class. Encapsulates the object that represents format3d in Go.'
## Format3D class
This class specifies the 3D shape properties for a chart element or shape.
```go
type Format3D struct  {
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
|[GetTopBevel](./gettopbevel/) | Gets the Bevel object that holds the properties associated with defining a bevel on the top or front face of a shape. |
|[HasTopBevelData](./hastopbeveldata/) | Indicates if the shape has top bevel data. |
|[GetSurfaceMaterialType](./getsurfacematerialtype/) | Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape.Default value is PresetMaterialType.WarmMatte. |
|[SetSurfaceMaterialType](./setsurfacematerialtype/) | Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape.Default value is PresetMaterialType.WarmMatte. |
|[GetSurfaceLightingType](./getsurfacelightingtype/) | Gets and sets the lighting type which is to be applied to the scene of the shape.Default value is LightRigType.ThreePoint. |
|[SetSurfaceLightingType](./setsurfacelightingtype/) | Gets and sets the lighting type which is to be applied to the scene of the shape.Default value is LightRigType.ThreePoint. |
|[GetLightingAngle](./getlightingangle/) | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
|[SetLightingAngle](./setlightingangle/) | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
