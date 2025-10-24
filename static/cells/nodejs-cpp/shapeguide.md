##ShapeGuide
Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape
## ShapeGuide class
Encapsulates a shape guide specifies the presence of a shape guide that will be used to govern the geometry of the specified shape
```javascript
class ShapeGuide extends BaseShapeGuide;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(BaseShapeGuide)](#constructor-baseshapeguide-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [value](#value--)| number | Gets or sets value of this guide |
## Methods
| Method | Description |
| --- | --- |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets value of this guide |
| [setValue(number)](#setValue-number-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets value of this guide |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(BaseShapeGuide) {#constructor-baseshapeguide-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: BaseShapeGuide);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | BaseShapeGuide | The parent object. |
### value {#value--}
Gets or sets value of this guide
```javascript
value : number;
```
### getValue() {#getValue--}
```javascript
getValue() : number;
```
### setValue(number) {#setValue-number-}
```javascript
setValue(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
