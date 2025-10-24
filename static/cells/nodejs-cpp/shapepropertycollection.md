##ShapePropertyCollection
This class specifies the visual shape properties for a chart element or shape.
## ShapePropertyCollection class
This class specifies the visual shape properties for a chart element or shape.
```javascript
class ShapePropertyCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [glowEffect](#glowEffect--)| GlowEffect | Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [format3D](#format3D--)| Format3D | Readonly. Represents a [Format3D](../format3d/) object that specifies 3D shape properties for the chart element or shape. |
| [softEdgeRadius](#softEdgeRadius--)| number | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [shadowEffect](#shadowEffect--)| ShadowEffect | Readonly. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
## Methods
| Method | Description |
| --- | --- |
| [getGlowEffect()](#getGlowEffect--)| <b>@deprecated.</b> Please use the 'glowEffect' property instead. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [getFormat3D()](#getFormat3D--)| <b>@deprecated.</b> Please use the 'format3D' property instead. Represents a [Format3D](../format3d/) object that specifies 3D shape properties for the chart element or shape. |
| [getSoftEdgeRadius()](#getSoftEdgeRadius--)| <b>@deprecated.</b> Please use the 'softEdgeRadius' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [setSoftEdgeRadius(number)](#setSoftEdgeRadius-number-)| <b>@deprecated.</b> Please use the 'softEdgeRadius' property instead. Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [getShadowEffect()](#getShadowEffect--)| <b>@deprecated.</b> Please use the 'shadowEffect' property instead. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [clearGlowEffect()](#clearGlowEffect--)| Clears the glow effect of the shape. |
| [hasGlowEffect()](#hasGlowEffect--)| Indicates if the shape has glow effect data. |
| [hasFormat3D()](#hasFormat3D--)| Indicates if the shape has 3d format data. |
| [clearFormat3D()](#clearFormat3D--)| Clears the 3D shape properties of the shape. |
| [clearShadowEffect()](#clearShadowEffect--)| Clears the shadow effect of the chart element or shape. |
| [hasShadowEffect()](#hasShadowEffect--)| Indicates if the shape has shadow effect data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### glowEffect {#glowEffect--}
Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape.
```javascript
glowEffect : GlowEffect;
```
### format3D {#format3D--}
Readonly. Represents a [Format3D](../format3d/) object that specifies 3D shape properties for the chart element or shape.
```javascript
format3D : Format3D;
```
### softEdgeRadius {#softEdgeRadius--}
Gets and sets the radius of blur to apply to the edges, in unit of points.
```javascript
softEdgeRadius : number;
```
### shadowEffect {#shadowEffect--}
Readonly. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape.
```javascript
shadowEffect : ShadowEffect;
```
### getGlowEffect() {#getGlowEffect--}
```javascript
getGlowEffect() : GlowEffect;
```
**Returns**
[GlowEffect](../gloweffect/)
### getFormat3D() {#getFormat3D--}
```javascript
getFormat3D() : Format3D;
```
**Returns**
[Format3D](../format3d/)
### getSoftEdgeRadius() {#getSoftEdgeRadius--}
```javascript
getSoftEdgeRadius() : number;
```
### setSoftEdgeRadius(number) {#setSoftEdgeRadius-number-}
```javascript
setSoftEdgeRadius(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getShadowEffect() {#getShadowEffect--}
```javascript
getShadowEffect() : ShadowEffect;
```
**Returns**
[ShadowEffect](../shadoweffect/)
### clearGlowEffect() {#clearGlowEffect--}
Clears the glow effect of the shape.
```javascript
clearGlowEffect() : void;
```
### hasGlowEffect() {#hasGlowEffect--}
Indicates if the shape has glow effect data.
```javascript
hasGlowEffect() : boolean;
```
### hasFormat3D() {#hasFormat3D--}
Indicates if the shape has 3d format data.
```javascript
hasFormat3D() : boolean;
```
### clearFormat3D() {#clearFormat3D--}
Clears the 3D shape properties of the shape.
```javascript
clearFormat3D() : void;
```
### clearShadowEffect() {#clearShadowEffect--}
Clears the shadow effect of the chart element or shape.
```javascript
clearShadowEffect() : void;
```
### hasShadowEffect() {#hasShadowEffect--}
Indicates if the shape has shadow effect data.
```javascript
hasShadowEffect() : boolean;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
