---
title: Format3D
second_title: Aspose.Cells for Node.js via C++ API Reference
description: This class specifies the 3D shape properties for a chart element or shape.
type: docs
url: /nodejs-cpp/format3d/
---

## Format3D class

This class specifies the 3D shape properties for a chart element or shape.

```javascript
class Format3D;
```


## Methods

| Method | Description |
| --- | --- |
| [getTopBevel()](#getTopBevel--)| Gets the [Bevel](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape. |
| [getSurfaceMaterialType()](#getSurfaceMaterialType--)| Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [setSurfaceMaterialType(PresetMaterialType)](#setSurfaceMaterialType-presetmaterialtype-)| Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [getSurfaceLightingType()](#getSurfaceLightingType--)| Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [setSurfaceLightingType(LightRigType)](#setSurfaceLightingType-lightrigtype-)| Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [getLightingAngle()](#getLightingAngle--)| Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [setLightingAngle(number)](#setLightingAngle-number-)| Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [hasTopBevelData()](#hasTopBevelData--)| Indicates if the shape has top bevel data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getTopBevel() {#getTopBevel--}

Gets the [Bevel](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape.

```javascript
getTopBevel() : Bevel;
```


**Returns**

[Bevel](../bevel/)

### getSurfaceMaterialType() {#getSurfaceMaterialType--}

Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte.

```javascript
getSurfaceMaterialType() : PresetMaterialType;
```


**Returns**

[PresetMaterialType](../presetmaterialtype/)

### setSurfaceMaterialType(PresetMaterialType) {#setSurfaceMaterialType-presetmaterialtype-}

Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte.

```javascript
setSurfaceMaterialType(value: PresetMaterialType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PresetMaterialType](../presetmaterialtype/) | The value to set. |

### getSurfaceLightingType() {#getSurfaceLightingType--}

Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint.

```javascript
getSurfaceLightingType() : LightRigType;
```


**Returns**

[LightRigType](../lightrigtype/)

### setSurfaceLightingType(LightRigType) {#setSurfaceLightingType-lightrigtype-}

Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint.

```javascript
setSurfaceLightingType(value: LightRigType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightRigType](../lightrigtype/) | The value to set. |

### getLightingAngle() {#getLightingAngle--}

Gets and sets the lighting angle. Range from 0 to 359.9 degrees.

```javascript
getLightingAngle() : number;
```


### setLightingAngle(number) {#setLightingAngle-number-}

Gets and sets the lighting angle. Range from 0 to 359.9 degrees.

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



