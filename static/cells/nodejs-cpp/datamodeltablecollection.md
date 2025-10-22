##DataModelTableCollection
Represents the list of the data model table.
## DataModelTableCollection class
Represents the list of the data model table.
```javascript
class DataModelTableCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the data model table by position of the collection. |
| [get(string)](#get-string-)| Gets the data model table by the name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the data model table by position of the collection.
```javascript
get(index: number) : DataModelTable;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position of the collection. |
**Returns**
[DataModelTable](../datamodeltable/)
### get(string) {#get-string-}
Gets the data model table by the name.
```javascript
get(name: string) : DataModelTable;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of data model table. |
**Returns**
[DataModelTable](../datamodeltable/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
