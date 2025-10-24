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
| [getHashCode()](#getHashCode--)| Gets hashcode. |
| [equals(VObject)](#equals-vobject-)|  |
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
### getHashCode() {#getHashCode--}
Gets hashcode.
```javascript
getHashCode() : number;
```
### equals(VObject) {#equals-vobject-}
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject |  |
