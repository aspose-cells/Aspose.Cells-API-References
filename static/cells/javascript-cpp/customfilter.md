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
| [criteria](#criteria--)| VObject | Gets and sets the criteria. |
## Methods
| Method | Description |
| --- | --- |
| [setCriteria(FilterOperatorType, VObject)](#setCriteria-filteroperatortype-vobject-)| Sets the filter criteria. |
### filterOperatorType {#filterOperatorType--}
Gets and sets the filter operator type.
```javascript
filterOperatorType : FilterOperatorType;
```
### criteria {#criteria--}
Gets and sets the criteria.
```javascript
criteria : VObject;
```
### setCriteria(FilterOperatorType, VObject) {#setCriteria-filteroperatortype-vobject-}
Sets the filter criteria.
```javascript
setCriteria(filterOperator: FilterOperatorType, criteria: VObject) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filterOperator | [FilterOperatorType](../filteroperatortype/) | filter operator type |
| criteria | VObject | filter criteria value |
