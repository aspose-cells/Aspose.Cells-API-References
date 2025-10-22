##RevisionCollection
Represents all revision logs.
## RevisionCollection class
Represents all revision logs.
```javascript
class RevisionCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [Revision](../revision/) by the index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets [Revision](../revision/) by the index.
```javascript
get(index: number) : Revision;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[Revision](../revision/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
