##SensitivityLabelCollection
Represents the list of sensitivity labels.
## SensitivityLabelCollection class
Represents the list of sensitivity labels.
```javascript
class SensitivityLabelCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [add(string, boolean, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType)](#add-string-boolean-sensitivitylabelassignmenttype-string-sensitivitylabelmarktype-)| Adds a sensitivity label. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### add(string, boolean, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType) {#add-string-boolean-sensitivitylabelassignmenttype-string-sensitivitylabelmarktype-}
Adds a sensitivity label.
```javascript
add(id: string, isEnabled: boolean, methodType: SensitivityLabelAssignmentType, siteId: string, markType: SensitivityLabelMarkType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | string | The id of the label. |
| isEnabled | boolean | Indicates whether this sensitivity label is enabled. |
| methodType | [SensitivityLabelAssignmentType](../sensitivitylabelassignmenttype/) | The assignment method type. |
| siteId | string | The id of the site. |
| markType | [SensitivityLabelMarkType](../sensitivitylabelmarktype/) | The mark type. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
