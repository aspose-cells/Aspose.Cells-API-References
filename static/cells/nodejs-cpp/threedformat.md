##ThreeDFormat
Represents a shapes threedimensional formatting.
## ThreeDFormat class
Represents a shape's three-dimensional formatting.
```javascript
class ThreeDFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [bottomBevelWidth](#bottomBevelWidth--)| number | Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [bottomBevelHeight](#bottomBevelHeight--)| number | Gets and sets the height of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [bottomBevelType](#bottomBevelType--)| BevelType | Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [topBevelWidth](#topBevelWidth--)| number | Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [topBevelHeight](#topBevelHeight--)| number | Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [topBevelType](#topBevelType--)| BevelType | Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [material](#material--)| PresetMaterialType | Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape. |
| [contourColor](#contourColor--)| CellsColor | Gets and sets the contour color on a shape. |
| [contourWidth](#contourWidth--)| number | Gets and sets the contour width on the shape, in unit of points. |
| [extrusionColor](#extrusionColor--)| CellsColor | Gets the extrusion color on a shape. |
| [extrusionHeight](#extrusionHeight--)| number | Gets and sets the extrusion height of the applied to the shape, in unit of points. |
| [z](#z--)| number | Defines the distance from ground for the 3D shape. |
| [lightAngle](#lightAngle--)| number | Gets and sets the angle of the extrusion lights. |
| [lighting](#lighting--)| LightRigType | Gets and sets type of light rig. |
| [lightingDirection](#lightingDirection--)| LightRigDirectionType | Gets and sets the direction from which the light rig is oriented in relation to the scene. |
| [perspective](#perspective--)| number | Gets and sets the angle at which a ThreeDFormat object can be viewed. |
| [rotationX](#rotationX--)| number | Gets and sets the rotation of the extruded shape around the x-axis in degrees. |
| [rotationY](#rotationY--)| number | Gets and sets the rotation of the extruded shape around the y-axis in degrees. |
| [rotationZ](#rotationZ--)| number | Gets and sets the rotation of the extruded shape around the z-axis in degrees. |
| [presetCameraType](#presetCameraType--)| PresetCameraType | Gets and sets the extrusion preset camera type. |
## Methods
| Method | Description |
| --- | --- |
| [getBottomBevelWidth()](#getBottomBevelWidth--)| <b>@deprecated.</b> Please use the 'bottomBevelWidth' property instead. Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [setBottomBevelWidth(number)](#setBottomBevelWidth-number-)| <b>@deprecated.</b> Please use the 'bottomBevelWidth' property instead. Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [getBottomBevelHeight()](#getBottomBevelHeight--)| <b>@deprecated.</b> Please use the 'bottomBevelHeight' property instead. Gets and sets the height of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [setBottomBevelHeight(number)](#setBottomBevelHeight-number-)| <b>@deprecated.</b> Please use the 'bottomBevelHeight' property instead. Gets and sets the height of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [getBottomBevelType()](#getBottomBevelType--)| <b>@deprecated.</b> Please use the 'bottomBevelType' property instead. Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [setBottomBevelType(BevelType)](#setBottomBevelType-beveltype-)| <b>@deprecated.</b> Please use the 'bottomBevelType' property instead. Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [getTopBevelWidth()](#getTopBevelWidth--)| <b>@deprecated.</b> Please use the 'topBevelWidth' property instead. Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [setTopBevelWidth(number)](#setTopBevelWidth-number-)| <b>@deprecated.</b> Please use the 'topBevelWidth' property instead. Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [getTopBevelHeight()](#getTopBevelHeight--)| <b>@deprecated.</b> Please use the 'topBevelHeight' property instead. Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [setTopBevelHeight(number)](#setTopBevelHeight-number-)| <b>@deprecated.</b> Please use the 'topBevelHeight' property instead. Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [getTopBevelType()](#getTopBevelType--)| <b>@deprecated.</b> Please use the 'topBevelType' property instead. Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [setTopBevelType(BevelType)](#setTopBevelType-beveltype-)| <b>@deprecated.</b> Please use the 'topBevelType' property instead. Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [getMaterial()](#getMaterial--)| <b>@deprecated.</b> Please use the 'material' property instead. Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape. |
| [setMaterial(PresetMaterialType)](#setMaterial-presetmaterialtype-)| <b>@deprecated.</b> Please use the 'material' property instead. Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape. |
| [getContourColor()](#getContourColor--)| <b>@deprecated.</b> Please use the 'contourColor' property instead. Gets and sets the contour color on a shape. |
| [setContourColor(CellsColor)](#setContourColor-cellscolor-)| <b>@deprecated.</b> Please use the 'contourColor' property instead. Gets and sets the contour color on a shape. |
| [getContourWidth()](#getContourWidth--)| <b>@deprecated.</b> Please use the 'contourWidth' property instead. Gets and sets the contour width on the shape, in unit of points. |
| [setContourWidth(number)](#setContourWidth-number-)| <b>@deprecated.</b> Please use the 'contourWidth' property instead. Gets and sets the contour width on the shape, in unit of points. |
| [getExtrusionColor()](#getExtrusionColor--)| <b>@deprecated.</b> Please use the 'extrusionColor' property instead. Gets the extrusion color on a shape. |
| [setExtrusionColor(CellsColor)](#setExtrusionColor-cellscolor-)| <b>@deprecated.</b> Please use the 'extrusionColor' property instead. Gets the extrusion color on a shape. |
| [getExtrusionHeight()](#getExtrusionHeight--)| <b>@deprecated.</b> Please use the 'extrusionHeight' property instead. Gets and sets the extrusion height of the applied to the shape, in unit of points. |
| [setExtrusionHeight(number)](#setExtrusionHeight-number-)| <b>@deprecated.</b> Please use the 'extrusionHeight' property instead. Gets and sets the extrusion height of the applied to the shape, in unit of points. |
| [getZ()](#getZ--)| <b>@deprecated.</b> Please use the 'z' property instead. Defines the distance from ground for the 3D shape. |
| [setZ(number)](#setZ-number-)| <b>@deprecated.</b> Please use the 'z' property instead. Defines the distance from ground for the 3D shape. |
| [getLightAngle()](#getLightAngle--)| <b>@deprecated.</b> Please use the 'lightAngle' property instead. Gets and sets the angle of the extrusion lights. |
| [setLightAngle(number)](#setLightAngle-number-)| <b>@deprecated.</b> Please use the 'lightAngle' property instead. Gets and sets the angle of the extrusion lights. |
| [getLighting()](#getLighting--)| <b>@deprecated.</b> Please use the 'lighting' property instead. Gets and sets type of light rig. |
| [setLighting(LightRigType)](#setLighting-lightrigtype-)| <b>@deprecated.</b> Please use the 'lighting' property instead. Gets and sets type of light rig. |
| [getLightingDirection()](#getLightingDirection--)| <b>@deprecated.</b> Please use the 'lightingDirection' property instead. Gets and sets the direction from which the light rig is oriented in relation to the scene. |
| [setLightingDirection(LightRigDirectionType)](#setLightingDirection-lightrigdirectiontype-)| <b>@deprecated.</b> Please use the 'lightingDirection' property instead. Gets and sets the direction from which the light rig is oriented in relation to the scene. |
| [getPerspective()](#getPerspective--)| <b>@deprecated.</b> Please use the 'perspective' property instead. Gets and sets the angle at which a ThreeDFormat object can be viewed. |
| [setPerspective(number)](#setPerspective-number-)| <b>@deprecated.</b> Please use the 'perspective' property instead. Gets and sets the angle at which a ThreeDFormat object can be viewed. |
| [getRotationX()](#getRotationX--)| <b>@deprecated.</b> Please use the 'rotationX' property instead. Gets and sets the rotation of the extruded shape around the x-axis in degrees. |
| [setRotationX(number)](#setRotationX-number-)| <b>@deprecated.</b> Please use the 'rotationX' property instead. Gets and sets the rotation of the extruded shape around the x-axis in degrees. |
| [getRotationY()](#getRotationY--)| <b>@deprecated.</b> Please use the 'rotationY' property instead. Gets and sets the rotation of the extruded shape around the y-axis in degrees. |
| [setRotationY(number)](#setRotationY-number-)| <b>@deprecated.</b> Please use the 'rotationY' property instead. Gets and sets the rotation of the extruded shape around the y-axis in degrees. |
| [getRotationZ()](#getRotationZ--)| <b>@deprecated.</b> Please use the 'rotationZ' property instead. Gets and sets the rotation of the extruded shape around the z-axis in degrees. |
| [setRotationZ(number)](#setRotationZ-number-)| <b>@deprecated.</b> Please use the 'rotationZ' property instead. Gets and sets the rotation of the extruded shape around the z-axis in degrees. |
| [getPresetCameraType()](#getPresetCameraType--)| <b>@deprecated.</b> Please use the 'presetCameraType' property instead. Gets and sets the extrusion preset camera type. |
| [setPresetCameraType(PresetCameraType)](#setPresetCameraType-presetcameratype-)| <b>@deprecated.</b> Please use the 'presetCameraType' property instead. Gets and sets the extrusion preset camera type. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getHashCode()](#getHashCode--)| Gets hashcode. |
| [equals(Object)](#equals-object-)|  |
### bottomBevelWidth {#bottomBevelWidth--}
Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points.
```javascript
bottomBevelWidth : number;
```
### bottomBevelHeight {#bottomBevelHeight--}
Gets and sets the height of the bottom bevel, or how far into the shape it is applied. In unit of Points.
```javascript
bottomBevelHeight : number;
```
### bottomBevelType {#bottomBevelType--}
Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points.
```javascript
bottomBevelType : BevelType;
```
### topBevelWidth {#topBevelWidth--}
Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points.
```javascript
topBevelWidth : number;
```
### topBevelHeight {#topBevelHeight--}
Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points.
```javascript
topBevelHeight : number;
```
### topBevelType {#topBevelType--}
Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points.
```javascript
topBevelType : BevelType;
```
### material {#material--}
Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape.
```javascript
material : PresetMaterialType;
```
### contourColor {#contourColor--}
Gets and sets the contour color on a shape.
```javascript
contourColor : CellsColor;
```
### contourWidth {#contourWidth--}
Gets and sets the contour width on the shape, in unit of points.
```javascript
contourWidth : number;
```
### extrusionColor {#extrusionColor--}
Gets the extrusion color on a shape.
```javascript
extrusionColor : CellsColor;
```
### extrusionHeight {#extrusionHeight--}
Gets and sets the extrusion height of the applied to the shape, in unit of points.
```javascript
extrusionHeight : number;
```
### z {#z--}
Defines the distance from ground for the 3D shape.
```javascript
z : number;
```
### lightAngle {#lightAngle--}
Gets and sets the angle of the extrusion lights.
```javascript
lightAngle : number;
```
### lighting {#lighting--}
Gets and sets type of light rig.
```javascript
lighting : LightRigType;
```
### lightingDirection {#lightingDirection--}
Gets and sets the direction from which the light rig is oriented in relation to the scene.
```javascript
lightingDirection : LightRigDirectionType;
```
### perspective {#perspective--}
Gets and sets the angle at which a ThreeDFormat object can be viewed.
```javascript
perspective : number;
```
### rotationX {#rotationX--}
Gets and sets the rotation of the extruded shape around the x-axis in degrees.
```javascript
rotationX : number;
```
### rotationY {#rotationY--}
Gets and sets the rotation of the extruded shape around the y-axis in degrees.
```javascript
rotationY : number;
```
### rotationZ {#rotationZ--}
Gets and sets the rotation of the extruded shape around the z-axis in degrees.
```javascript
rotationZ : number;
```
### presetCameraType {#presetCameraType--}
Gets and sets the extrusion preset camera type.
```javascript
presetCameraType : PresetCameraType;
```
### getBottomBevelWidth() {#getBottomBevelWidth--}
```javascript
getBottomBevelWidth() : number;
```
### setBottomBevelWidth(number) {#setBottomBevelWidth-number-}
```javascript
setBottomBevelWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBottomBevelHeight() {#getBottomBevelHeight--}
```javascript
getBottomBevelHeight() : number;
```
### setBottomBevelHeight(number) {#setBottomBevelHeight-number-}
```javascript
setBottomBevelHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBottomBevelType() {#getBottomBevelType--}
```javascript
getBottomBevelType() : BevelType;
```
**Returns**
[BevelType](../beveltype/)
### setBottomBevelType(BevelType) {#setBottomBevelType-beveltype-}
```javascript
setBottomBevelType(value: BevelType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BevelType](../beveltype/) | The value to set. |
### getTopBevelWidth() {#getTopBevelWidth--}
```javascript
getTopBevelWidth() : number;
```
### setTopBevelWidth(number) {#setTopBevelWidth-number-}
```javascript
setTopBevelWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTopBevelHeight() {#getTopBevelHeight--}
```javascript
getTopBevelHeight() : number;
```
### setTopBevelHeight(number) {#setTopBevelHeight-number-}
```javascript
setTopBevelHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTopBevelType() {#getTopBevelType--}
```javascript
getTopBevelType() : BevelType;
```
**Returns**
[BevelType](../beveltype/)
### setTopBevelType(BevelType) {#setTopBevelType-beveltype-}
```javascript
setTopBevelType(value: BevelType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BevelType](../beveltype/) | The value to set. |
### getMaterial() {#getMaterial--}
```javascript
getMaterial() : PresetMaterialType;
```
**Returns**
[PresetMaterialType](../presetmaterialtype/)
### setMaterial(PresetMaterialType) {#setMaterial-presetmaterialtype-}
```javascript
setMaterial(value: PresetMaterialType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PresetMaterialType](../presetmaterialtype/) | The value to set. |
### getContourColor() {#getContourColor--}
```javascript
getContourColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setContourColor(CellsColor) {#setContourColor-cellscolor-}
```javascript
setContourColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
### getContourWidth() {#getContourWidth--}
```javascript
getContourWidth() : number;
```
### setContourWidth(number) {#setContourWidth-number-}
```javascript
setContourWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getExtrusionColor() {#getExtrusionColor--}
```javascript
getExtrusionColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setExtrusionColor(CellsColor) {#setExtrusionColor-cellscolor-}
```javascript
setExtrusionColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
### getExtrusionHeight() {#getExtrusionHeight--}
```javascript
getExtrusionHeight() : number;
```
### setExtrusionHeight(number) {#setExtrusionHeight-number-}
```javascript
setExtrusionHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getZ() {#getZ--}
```javascript
getZ() : number;
```
### setZ(number) {#setZ-number-}
```javascript
setZ(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLightAngle() {#getLightAngle--}
```javascript
getLightAngle() : number;
```
### setLightAngle(number) {#setLightAngle-number-}
```javascript
setLightAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLighting() {#getLighting--}
```javascript
getLighting() : LightRigType;
```
**Returns**
[LightRigType](../lightrigtype/)
### setLighting(LightRigType) {#setLighting-lightrigtype-}
```javascript
setLighting(value: LightRigType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightRigType](../lightrigtype/) | The value to set. |
### getLightingDirection() {#getLightingDirection--}
```javascript
getLightingDirection() : LightRigDirectionType;
```
**Returns**
[LightRigDirectionType](../lightrigdirectiontype/)
### setLightingDirection(LightRigDirectionType) {#setLightingDirection-lightrigdirectiontype-}
```javascript
setLightingDirection(value: LightRigDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightRigDirectionType](../lightrigdirectiontype/) | The value to set. |
### getPerspective() {#getPerspective--}
```javascript
getPerspective() : number;
```
### setPerspective(number) {#setPerspective-number-}
```javascript
setPerspective(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRotationX() {#getRotationX--}
```javascript
getRotationX() : number;
```
### setRotationX(number) {#setRotationX-number-}
```javascript
setRotationX(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRotationY() {#getRotationY--}
```javascript
getRotationY() : number;
```
### setRotationY(number) {#setRotationY-number-}
```javascript
setRotationY(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRotationZ() {#getRotationZ--}
```javascript
getRotationZ() : number;
```
### setRotationZ(number) {#setRotationZ-number-}
```javascript
setRotationZ(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPresetCameraType() {#getPresetCameraType--}
```javascript
getPresetCameraType() : PresetCameraType;
```
**Returns**
[PresetCameraType](../presetcameratype/)
### setPresetCameraType(PresetCameraType) {#setPresetCameraType-presetcameratype-}
```javascript
setPresetCameraType(value: PresetCameraType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PresetCameraType](../presetcameratype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getHashCode() {#getHashCode--}
Gets hashcode.
```javascript
getHashCode() : number;
```
### equals(Object) {#equals-object-}
```javascript
equals(obj: Object) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
