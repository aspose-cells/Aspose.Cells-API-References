##TextTabStopCollection
Represents the list of all tab stops.
## TextTabStopCollection class
Represents the list of all tab stops.
```javascript
class TextTabStopCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [TextTabStop](../texttabstop/) by the index. |
| [add(TextTabAlignmentType, number)](#add-texttabalignmenttype-number-)| Adds a tab stop. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets [TextTabStop](../texttabstop/) by the index.
```javascript
get(index: number) : TextTabStop;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[TextTabStop](../texttabstop/)
### add(TextTabAlignmentType, number) {#add-texttabalignmenttype-number-}
Adds a tab stop.
```javascript
add(tabAlignment: TextTabAlignmentType, tabPosition: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tabAlignment | [TextTabAlignmentType](../texttabalignmenttype/) |  |
| tabPosition | number |  |
