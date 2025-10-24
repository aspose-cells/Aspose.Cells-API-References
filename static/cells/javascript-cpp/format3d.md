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
| [hasTopBevelData()](#hasTopBevelData--)| Indicates if the shape has top bevel data. |
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
### hasTopBevelData() {#hasTopBevelData--}
Indicates if the shape has top bevel data.
```javascript
hasTopBevelData() : boolean;
```
