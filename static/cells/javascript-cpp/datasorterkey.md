##DataSorterKey
Represents the key of the data sorter.
## DataSorterKey class
Represents the key of the data sorter.
```javascript
class DataSorterKey;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [order](#order--)| SortOrder | Readonly. Indicates the order of sorting. |
| [index](#index--)| number | Readonly. Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [type](#type--)| SortOnType | Readonly. Represents the type of sorting. |
| [iconSetType](#iconSetType--)| IconSetType | Readonly. Represents the icon set type. |
| [iconId](#iconId--)| number | Readonly. Represents the id of the icon set type. |
| [color](#color--)| Color | Readonly. Gets the sorted color. |
### order {#order--}
Readonly. Indicates the order of sorting.
```javascript
order : SortOrder;
```
### index {#index--}
Readonly. Gets the sorted column index(absolute position, column A is 0, B is 1, ...).
```javascript
index : number;
```
### type {#type--}
Readonly. Represents the type of sorting.
```javascript
type : SortOnType;
```
### iconSetType {#iconSetType--}
Readonly. Represents the icon set type.
```javascript
iconSetType : IconSetType;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### iconId {#iconId--}
Readonly. Represents the id of the icon set type.
```javascript
iconId : number;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### color {#color--}
Readonly. Gets the sorted color.
```javascript
color : Color;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.CellColor](../sortontype.cellcolor/) or [SortOnType.FontColor](../sortontype.fontcolor/).
