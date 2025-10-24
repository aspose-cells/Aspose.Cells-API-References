##QueryTableCollection
A collection of QueryTableCollection..querytablecollection objects that represent QueryTable collection information.
## QueryTableCollection class
A collection of [QueryTableCollection](../querytablecollection/) objects that represent QueryTable collection information.
```javascript
class QueryTableCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the querytable by the specific index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the querytable by the specific index.
```javascript
get(index: number) : QueryTable;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The querytable
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
