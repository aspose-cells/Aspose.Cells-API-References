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
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the preset reflection effect. |
| [setType(ReflectionEffectType)](#setType-reflectioneffecttype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the preset reflection effect. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
| [setSize(number)](#setSize-number-)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
| [getBlur()](#getBlur--)| <b>@deprecated.</b> Please use the 'blur' property instead. Gets and sets the blur radius,in unit of points. |
| [setBlur(number)](#setBlur-number-)| <b>@deprecated.</b> Please use the 'blur' property instead. Gets and sets the blur radius,in unit of points. |
| [getDirection()](#getDirection--)| <b>@deprecated.</b> Please use the 'direction' property instead. Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
| [setDirection(number)](#setDirection-number-)| <b>@deprecated.</b> Please use the 'direction' property instead. Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
| [getDistance()](#getDistance--)| <b>@deprecated.</b> Please use the 'distance' property instead. Gets and sets how far to distance the shadow,in unit of points. |
| [setDistance(number)](#setDistance-number-)| <b>@deprecated.</b> Please use the 'distance' property instead. Gets and sets how far to distance the shadow,in unit of points. |
| [getFadeDirection()](#getFadeDirection--)| <b>@deprecated.</b> Please use the 'fadeDirection' property instead. Gets and sets the direction to offset the reflection. |
| [setFadeDirection(number)](#setFadeDirection-number-)| <b>@deprecated.</b> Please use the 'fadeDirection' property instead. Gets and sets the direction to offset the reflection. |
| [getRotWithShape()](#getRotWithShape--)| <b>@deprecated.</b> Please use the 'rotWithShape' property instead. Gets and sets if the reflection should rotate with the shape. |
| [setRotWithShape(boolean)](#setRotWithShape-boolean-)| <b>@deprecated.</b> Please use the 'rotWithShape' property instead. Gets and sets if the reflection should rotate with the shape. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getType() {#getType--}
```javascript
getType() : ReflectionEffectType;
```
**Returns**
[ReflectionEffectType](../reflectioneffecttype/)
### setType(ReflectionEffectType) {#setType-reflectioneffecttype-}
```javascript
setType(value: ReflectionEffectType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReflectionEffectType](../reflectioneffecttype/) | The value to set. |
### getTransparency() {#getTransparency--}
```javascript
getTransparency() : number;
```
### setTransparency(number) {#setTransparency-number-}
```javascript
setTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSize() {#getSize--}
```javascript
getSize() : number;
```
### setSize(number) {#setSize-number-}
```javascript
setSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBlur() {#getBlur--}
```javascript
getBlur() : number;
```
### setBlur(number) {#setBlur-number-}
```javascript
setBlur(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDirection() {#getDirection--}
```javascript
getDirection() : number;
```
### setDirection(number) {#setDirection-number-}
```javascript
setDirection(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDistance() {#getDistance--}
```javascript
getDistance() : number;
```
### setDistance(number) {#setDistance-number-}
```javascript
setDistance(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFadeDirection() {#getFadeDirection--}
```javascript
getFadeDirection() : number;
```
### setFadeDirection(number) {#setFadeDirection-number-}
```javascript
setFadeDirection(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRotWithShape() {#getRotWithShape--}
```javascript
getRotWithShape() : boolean;
```
### setRotWithShape(boolean) {#setRotWithShape-boolean-}
```javascript
setRotWithShape(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
