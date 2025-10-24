##SensitivityLabelCollection
Represents the list of sensitivity labels.
## SensitivityLabelCollection class
Represents the list of sensitivity labels.
```javascript
class SensitivityLabelCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [add(string, boolean, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType)](#add-string-boolean-sensitivitylabelassignmenttype-string-sensitivitylabelmarktype-)| Adds a sensitivity label. |
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
