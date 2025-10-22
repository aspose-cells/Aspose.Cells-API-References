##ShapePathPointCollection
Represents all shape path points.
## ShapePathPointCollection class
Represents all shape path points.
```javascript
class ShapePathPointCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets shape path point by index. |
| [add(number, number)](#add-number-number-)| Adds a path point in unit of EMUs. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets shape path point by index.
```javascript
get(index: number) : ShapePathPoint;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |
**Returns**
Returns [ShapePathPoint](../shapepathpoint/) object
### add(number, number) {#add-number-number-}
Adds a path point in unit of EMUs.
```javascript
add(x: number, y: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | number | The x coordinate. |
| y | number | The y coordinate. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath. This method will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
