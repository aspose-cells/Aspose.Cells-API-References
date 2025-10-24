##ReflectionEffect
This class specifies a reflection effect.
## ReflectionEffect class
This class specifies a reflection effect.
```javascript
class ReflectionEffect;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| ReflectionEffectType | Gets and sets the preset reflection effect. |
| [transparency](#transparency--)| number | Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [size](#size--)| number | Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
| [blur](#blur--)| number | Gets and sets the blur radius,in unit of points. |
| [direction](#direction--)| number | Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
| [distance](#distance--)| number | Gets and sets how far to distance the shadow,in unit of points. |
| [fadeDirection](#fadeDirection--)| number | Gets and sets the direction to offset the reflection. |
| [rotWithShape](#rotWithShape--)| boolean | Gets and sets if the reflection should rotate with the shape. |
### type {#type--}
Gets and sets the preset reflection effect.
```javascript
type : ReflectionEffectType;
```
### transparency {#transparency--}
Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### size {#size--}
Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage
```javascript
size : number;
```
### blur {#blur--}
Gets and sets the blur radius,in unit of points.
```javascript
blur : number;
```
### direction {#direction--}
Gets and sets the direction of the alpha gradient ramp relative to the shape itself.
```javascript
direction : number;
```
### distance {#distance--}
Gets and sets how far to distance the shadow,in unit of points.
```javascript
distance : number;
```
### fadeDirection {#fadeDirection--}
Gets and sets the direction to offset the reflection.
```javascript
fadeDirection : number;
```
### rotWithShape {#rotWithShape--}
Gets and sets if the reflection should rotate with the shape.
```javascript
rotWithShape : boolean;
```
