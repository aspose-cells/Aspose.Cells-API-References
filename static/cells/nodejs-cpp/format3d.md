##Format3D
This class specifies the 3D shape properties for a chart element or shape.
## Format3D class
This class specifies the 3D shape properties for a chart element or shape.
```javascript
class Format3D;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [topBevel](#topBevel--)| Bevel | Readonly. Gets the [Bevel](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape. |
| [surfaceMaterialType](#surfaceMaterialType--)| PresetMaterialType | Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [surfaceLightingType](#surfaceLightingType--)| LightRigType | Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [lightingAngle](#lightingAngle--)| number | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
## Methods
| Method | Description |
| --- | --- |
| [getTopBevel()](#getTopBevel--)| <b>@deprecated.</b> Please use the 'topBevel' property instead. Gets the [Bevel](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape. |
| [getSurfaceMaterialType()](#getSurfaceMaterialType--)| <b>@deprecated.</b> Please use the 'surfaceMaterialType' property instead. Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [setSurfaceMaterialType(PresetMaterialType)](#setSurfaceMaterialType-presetmaterialtype-)| <b>@deprecated.</b> Please use the 'surfaceMaterialType' property instead. Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [getSurfaceLightingType()](#getSurfaceLightingType--)| <b>@deprecated.</b> Please use the 'surfaceLightingType' property instead. Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [setSurfaceLightingType(LightRigType)](#setSurfaceLightingType-lightrigtype-)| <b>@deprecated.</b> Please use the 'surfaceLightingType' property instead. Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [getLightingAngle()](#getLightingAngle--)| <b>@deprecated.</b> Please use the 'lightingAngle' property instead. Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [setLightingAngle(number)](#setLightingAngle-number-)| <b>@deprecated.</b> Please use the 'lightingAngle' property instead. Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [hasTopBevelData()](#hasTopBevelData--)| Indicates if the shape has top bevel data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### topBevel {#topBevel--}
Readonly. Gets the [Bevel](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape.
```javascript
topBevel : Bevel;
```
### surfaceMaterialType {#surfaceMaterialType--}
Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte.
```javascript
surfaceMaterialType : PresetMaterialType;
```
### surfaceLightingType {#surfaceLightingType--}
Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint.
```javascript
surfaceLightingType : LightRigType;
```
### lightingAngle {#lightingAngle--}
Gets and sets the lighting angle. Range from 0 to 359.9 degrees.
```javascript
lightingAngle : number;
```
### getTopBevel() {#getTopBevel--}
```javascript
getTopBevel() : Bevel;
```
**Returns**
[Bevel](../bevel/)
### getSurfaceMaterialType() {#getSurfaceMaterialType--}
```javascript
getSurfaceMaterialType() : PresetMaterialType;
```
**Returns**
[PresetMaterialType](../presetmaterialtype/)
### setSurfaceMaterialType(PresetMaterialType) {#setSurfaceMaterialType-presetmaterialtype-}
```javascript
setSurfaceMaterialType(value: PresetMaterialType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PresetMaterialType](../presetmaterialtype/) | The value to set. |
### getSurfaceLightingType() {#getSurfaceLightingType--}
```javascript
getSurfaceLightingType() : LightRigType;
```
**Returns**
[LightRigType](../lightrigtype/)
### setSurfaceLightingType(LightRigType) {#setSurfaceLightingType-lightrigtype-}
```javascript
setSurfaceLightingType(value: LightRigType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightRigType](../lightrigtype/) | The value to set. |
### getLightingAngle() {#getLightingAngle--}
```javascript
getLightingAngle() : number;
```
### setLightingAngle(number) {#setLightingAngle-number-}
```javascript
setLightingAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### hasTopBevelData() {#hasTopBevelData--}
Indicates if the shape has top bevel data.
```javascript
hasTopBevelData() : boolean;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
