##CustomRenderSettings
Represents custom settings during rendering.
## CustomRenderSettings class
Represents custom settings during rendering.
```javascript
class CustomRenderSettings;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |
## Methods
| Method | Description |
| --- | --- |
| [getCellBorderWidth(CellBorderType)](#getCellBorderWidth-cellbordertype-)| Specifies cell border width according to border type. |
### constructor() {#constructor--}
Ctor.
```javascript
constructor();
```
### getCellBorderWidth(CellBorderType) {#getCellBorderWidth-cellbordertype-}
Specifies cell border width according to border type.
```javascript
getCellBorderWidth(borderType: CellBorderType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [CellBorderType](../cellbordertype/) | cell border type |
**Returns**
cell border width
**Remarks**
Any negative value will be ignored.
