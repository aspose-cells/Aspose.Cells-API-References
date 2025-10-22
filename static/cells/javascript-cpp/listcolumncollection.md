##ListColumnCollection
Represents A collection of all the ListColumn..listcolumn objects in the specified ListObject object.
## ListColumnCollection class
Represents A collection of all the [ListColumn](../listcolumn/) objects in the specified ListObject object.
```javascript
class ListColumnCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the ListColumn by the index. |
| [get(string)](#get-string-)| Gets the ListColumn by the name. |
### get(number) {#get-number-}
Gets the ListColumn by the index.
```javascript
get(index: number) : ListColumn;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
the ListColumn object.
### get(string) {#get-string-}
Gets the ListColumn by the name.
```javascript
get(name: string) : ListColumn;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the ListColumn |
**Returns**
The ListColumn object.
