##FilterColumn
Represents a filter for a single column. The Filter object is a member of the Filters collection
## FilterColumn class
Represents a filter for a single column. The Filter object is a member of the Filters collection
```javascript
class FilterColumn;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isDropdownVisible](#isDropdownVisible--)| boolean | Indicates whether the AutoFilter button for this column is visible. |
| [filter](#filter--)| Object | Gets and sets the condition of filtering data. |
| [filterType](#filterType--)| FilterType | Gets and sets the type fo filtering data. |
| [fieldIndex](#fieldIndex--)| number | Gets and sets the column offset in the range. |
## Methods
| Method | Description |
| --- | --- |
| [isDropdownVisible()](#isDropdownVisible--)| <b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible. |
| [setIsDropdownVisible(boolean)](#setIsDropdownVisible-boolean-)| <b>@deprecated.</b> Please use the 'isDropdownVisible' property instead. Indicates whether the AutoFilter button for this column is visible. |
| [getFilter()](#getFilter--)| <b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data. |
| [setFilter(Object)](#setFilter-object-)| <b>@deprecated.</b> Please use the 'filter' property instead. Gets and sets the condition of filtering data. |
| [getFilterType()](#getFilterType--)| <b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data. |
| [setFilterType(FilterType)](#setFilterType-filtertype-)| <b>@deprecated.</b> Please use the 'filterType' property instead. Gets and sets the type fo filtering data. |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
| [setFieldIndex(number)](#setFieldIndex-number-)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets and sets the column offset in the range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### isDropdownVisible {#isDropdownVisible--}
Indicates whether the AutoFilter button for this column is visible.
```javascript
isDropdownVisible : boolean;
```
### filter {#filter--}
Gets and sets the condition of filtering data.
```javascript
filter : Object;
```
### filterType {#filterType--}
Gets and sets the type fo filtering data.
```javascript
filterType : FilterType;
```
### fieldIndex {#fieldIndex--}
Gets and sets the column offset in the range.
```javascript
fieldIndex : number;
```
### isDropdownVisible() {#isDropdownVisible--}
```javascript
isDropdownVisible() : boolean;
```
### setIsDropdownVisible(boolean) {#setIsDropdownVisible-boolean-}
```javascript
setIsDropdownVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFilter() {#getFilter--}
```javascript
getFilter() : Object;
```
### setFilter(Object) {#setFilter-object-}
```javascript
setFilter(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### getFilterType() {#getFilterType--}
```javascript
getFilterType() : FilterType;
```
**Returns**
[FilterType](../filtertype/)
### setFilterType(FilterType) {#setFilterType-filtertype-}
```javascript
setFilterType(value: FilterType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FilterType](../filtertype/) | The value to set. |
### getFieldIndex() {#getFieldIndex--}
```javascript
getFieldIndex() : number;
```
### setFieldIndex(number) {#setFieldIndex-number-}
```javascript
setFieldIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
