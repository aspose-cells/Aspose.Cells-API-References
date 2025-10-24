##SmartTagSetting
Represents all SmartTagCollection..smarttagcollection object in the worksheet.
## SmartTagSetting class
Represents all [SmartTagCollection](../smarttagcollection/) object in the worksheet.
```javascript
class SmartTagSetting;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTagCollection](../smarttagcollection/) object by the index. |
| [get(number, number)](#get-number-number-)| Gets the [SmartTagCollection](../smarttagcollection/) object of the cell. |
| [get(string)](#get-string-)| Gets the [SmartTagCollection](../smarttagcollection/) object of the cell. |
| [add(number, number)](#add-number-number-)| Adds a [SmartTagCollection](../smarttagcollection/) object to a cell. |
| [add(string)](#add-string-)| Add a cell smart tags. |
### get(number) {#get-number-}
Gets a [SmartTagCollection](../smarttagcollection/) object by the index.
```javascript
get(index: number) : SmartTagCollection;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the [SmartTagCollection](../smarttagcollection/) object in the list. |
**Returns**
[SmartTagCollection](../smarttagcollection/)
### get(number, number) {#get-number-number-}
Gets the [SmartTagCollection](../smarttagcollection/) object of the cell.
```javascript
get(row: number, column: number) : SmartTagCollection;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index of the cell. |
| column | number | The column index of the cell |
**Returns**
Returns the [SmartTagCollection](../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.
### get(string) {#get-string-}
Gets the [SmartTagCollection](../smarttagcollection/) object of the cell.
```javascript
get(cellName: string) : SmartTagCollection;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |
**Returns**
Returns the [SmartTagCollection](../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.
### add(number, number) {#add-number-number-}
Adds a [SmartTagCollection](../smarttagcollection/) object to a cell.
```javascript
add(row: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row of the cell. |
| column | number | The column of the cell. |
**Returns**
Returns index of a [SmartTagCollection](../smarttagcollection/) object in the worksheet.
### add(string) {#add-string-}
Add a cell smart tags.
```javascript
add(cellName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |
