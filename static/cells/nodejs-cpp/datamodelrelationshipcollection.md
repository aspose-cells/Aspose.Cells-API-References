##DataModelRelationshipCollection
Represents the relationships.
## DataModelRelationshipCollection class
Represents the relationships.
```javascript
class DataModelRelationshipCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the relationship. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the relationship.
```javascript
get(index: number) : DataModelRelationship;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[DataModelRelationship](../datamodelrelationship/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
