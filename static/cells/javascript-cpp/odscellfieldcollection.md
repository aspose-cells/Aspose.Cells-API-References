##OdsCellFieldCollection
Represents the fields of ODS.
## OdsCellFieldCollection class
Represents the fields of ODS.
```javascript
class OdsCellFieldCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the field by the index. |
| [get(number, number)](#get-number-number-)| Gets the field by row and column index. |
| [add(number, number, OdsCellFieldType, string)](#add-number-number-odscellfieldtype-string-)| Adds a field. |
| [updateFieldsValue()](#updateFieldsValue--)| Update fields value to the cells. |
### get(number) {#get-number-}
Gets the field by the index.
```javascript
get(index: number) : OdsCellField;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[OdsCellField](../odscellfield/)
### get(number, number) {#get-number-number-}
Gets the field by row and column index.
```javascript
get(row: number, column: number) : OdsCellField;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
[OdsCellField](../odscellfield/)
### add(number, number, OdsCellFieldType, string) {#add-number-number-odscellfieldtype-string-}
Adds a field.
```javascript
add(row: number, column: number, fieldType: OdsCellFieldType, format: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
| fieldType | [OdsCellFieldType](../odscellfieldtype/) | The type of the field. |
| format | string | The number format of the field. |
### updateFieldsValue() {#updateFieldsValue--}
Update fields value to the cells.
```javascript
updateFieldsValue() : void;
```
