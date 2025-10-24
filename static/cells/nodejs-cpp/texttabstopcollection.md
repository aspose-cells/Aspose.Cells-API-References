##TextTabStopCollection
Represents the list of all tab stops.
## TextTabStopCollection class
Represents the list of all tab stops.
```javascript
class TextTabStopCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [TextTabStop](../texttabstop/) by the index. |
| [add(TextTabAlignmentType, number)](#add-texttabalignmenttype-number-)| Adds a tab stop. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
