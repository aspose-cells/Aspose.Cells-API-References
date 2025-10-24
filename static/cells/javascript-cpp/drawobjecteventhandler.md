##DrawObjectEventHandler
Interface to get DrawObject and Bound when rendering.
## DrawObjectEventHandler class
Interface to get DrawObject and Bound when rendering.
```javascript
abstract class DrawObjectEventHandler;
```
## Methods
| Method | Description |
| --- | --- |
| abstract [draw(DrawObject, number, number, number, number)](#draw-drawobject-number-number-number-number-)| Implements this interface to get DrawObject and Bound when rendering. |
### draw(DrawObject, number, number, number, number) {#draw-drawobject-number-number-number-number-}
Implements this interface to get DrawObject and Bound when rendering.
```javascript
abstract draw(drawObject: DrawObject, x: number, y: number, width: number, height: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| drawObject | [DrawObject](../drawobject/) | DrawObject will be initialized and returned when rendering |
| x | number | Left of DrawObject |
| y | number | Top of DrawObject |
| width | number | Width of DrawObject |
| height | number | Height of DrawObject |
