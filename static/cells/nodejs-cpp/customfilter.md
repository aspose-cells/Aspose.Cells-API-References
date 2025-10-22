##CustomFilter
Represents the custom filter.
## CustomFilter class
Represents the custom filter.
```javascript
class CustomFilter;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [filterOperatorType](#filterOperatorType--)| FilterOperatorType | Gets and sets the filter operator type. |
| [criteria](#criteria--)| Object | Gets and sets the criteria. |
## Methods
| Method | Description |
| --- | --- |
| [getFilterOperatorType()](#getFilterOperatorType--)| <b>@deprecated.</b> Please use the 'filterOperatorType' property instead. Gets and sets the filter operator type. |
| [setFilterOperatorType(FilterOperatorType)](#setFilterOperatorType-filteroperatortype-)| <b>@deprecated.</b> Please use the 'filterOperatorType' property instead. Gets and sets the filter operator type. |
| [getCriteria()](#getCriteria--)| <b>@deprecated.</b> Please use the 'criteria' property instead. Gets and sets the criteria. |
| [setCriteria(Object)](#setCriteria-object-)| <b>@deprecated.</b> Please use the 'criteria' property instead. Gets and sets the criteria. |
| [setCriteria(FilterOperatorType, Object)](#setCriteria-filteroperatortype-object-)| Sets the filter criteria. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### filterOperatorType {#filterOperatorType--}
Gets and sets the filter operator type.
```javascript
filterOperatorType : FilterOperatorType;
```
### criteria {#criteria--}
Gets and sets the criteria.
```javascript
criteria : Object;
```
### getFilterOperatorType() {#getFilterOperatorType--}
```javascript
getFilterOperatorType() : FilterOperatorType;
```
**Returns**
[FilterOperatorType](../filteroperatortype/)
### setFilterOperatorType(FilterOperatorType) {#setFilterOperatorType-filteroperatortype-}
```javascript
setFilterOperatorType(value: FilterOperatorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FilterOperatorType](../filteroperatortype/) | The value to set. |
### getCriteria() {#getCriteria--}
```javascript
getCriteria() : Object;
```
### setCriteria(Object) {#setCriteria-object-}
```javascript
setCriteria(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### setCriteria(FilterOperatorType, Object) {#setCriteria-filteroperatortype-object-}
Sets the filter criteria.
```javascript
setCriteria(filterOperator: FilterOperatorType, criteria: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filterOperator | [FilterOperatorType](../filteroperatortype/) | filter operator type |
| criteria | Object | filter criteria value |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
