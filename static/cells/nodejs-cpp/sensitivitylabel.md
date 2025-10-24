##SensitivityLabel
Represents the sensitivity label.
## SensitivityLabel class
Represents the sensitivity label.
```javascript
class SensitivityLabel;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [id](#id--)| string | Gets and sets the id of sensitivity label. |
| [isEnabled](#isEnabled--)| boolean | Indicates whether the sensitivity label is enabled |
| [assignmentType](#assignmentType--)| SensitivityLabelAssignmentType | Gets and sets the assignment method for the sensitivity label. |
| [siteId](#siteId--)| string | Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label. |
| [contentMarkType](#contentMarkType--)| SensitivityLabelMarkType | Gets and sets the types of content marking that ought to be applied to a file. |
| [isRemoved](#isRemoved--)| boolean | Indicates whether the sensitivity label was removed. |
## Methods
| Method | Description |
| --- | --- |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the id of sensitivity label. |
| [setId(string)](#setId-string-)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the id of sensitivity label. |
| [isEnabled()](#isEnabled--)| <b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the sensitivity label is enabled |
| [setIsEnabled(boolean)](#setIsEnabled-boolean-)| <b>@deprecated.</b> Please use the 'isEnabled' property instead. Indicates whether the sensitivity label is enabled |
| [getAssignmentType()](#getAssignmentType--)| <b>@deprecated.</b> Please use the 'assignmentType' property instead. Gets and sets the assignment method for the sensitivity label. |
| [setAssignmentType(SensitivityLabelAssignmentType)](#setAssignmentType-sensitivitylabelassignmenttype-)| <b>@deprecated.</b> Please use the 'assignmentType' property instead. Gets and sets the assignment method for the sensitivity label. |
| [getSiteId()](#getSiteId--)| <b>@deprecated.</b> Please use the 'siteId' property instead. Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label. |
| [setSiteId(string)](#setSiteId-string-)| <b>@deprecated.</b> Please use the 'siteId' property instead. Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label. |
| [getContentMarkType()](#getContentMarkType--)| <b>@deprecated.</b> Please use the 'contentMarkType' property instead. Gets and sets the types of content marking that ought to be applied to a file. |
| [setContentMarkType(SensitivityLabelMarkType)](#setContentMarkType-sensitivitylabelmarktype-)| <b>@deprecated.</b> Please use the 'contentMarkType' property instead. Gets and sets the types of content marking that ought to be applied to a file. |
| [isRemoved()](#isRemoved--)| <b>@deprecated.</b> Please use the 'isRemoved' property instead. Indicates whether the sensitivity label was removed. |
| [setIsRemoved(boolean)](#setIsRemoved-boolean-)| <b>@deprecated.</b> Please use the 'isRemoved' property instead. Indicates whether the sensitivity label was removed. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### id {#id--}
Gets and sets the id of sensitivity label.
```javascript
id : string;
```
### isEnabled {#isEnabled--}
Indicates whether the sensitivity label is enabled
```javascript
isEnabled : boolean;
```
### assignmentType {#assignmentType--}
Gets and sets the assignment method for the sensitivity label.
```javascript
assignmentType : SensitivityLabelAssignmentType;
```
### siteId {#siteId--}
Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label.
```javascript
siteId : string;
```
### contentMarkType {#contentMarkType--}
Gets and sets the types of content marking that ought to be applied to a file.
```javascript
contentMarkType : SensitivityLabelMarkType;
```
### isRemoved {#isRemoved--}
Indicates whether the sensitivity label was removed.
```javascript
isRemoved : boolean;
```
### getId() {#getId--}
```javascript
getId() : string;
```
### setId(string) {#setId-string-}
```javascript
setId(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isEnabled() {#isEnabled--}
```javascript
isEnabled() : boolean;
```
### setIsEnabled(boolean) {#setIsEnabled-boolean-}
```javascript
setIsEnabled(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAssignmentType() {#getAssignmentType--}
```javascript
getAssignmentType() : SensitivityLabelAssignmentType;
```
**Returns**
[SensitivityLabelAssignmentType](../sensitivitylabelassignmenttype/)
### setAssignmentType(SensitivityLabelAssignmentType) {#setAssignmentType-sensitivitylabelassignmenttype-}
```javascript
setAssignmentType(value: SensitivityLabelAssignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SensitivityLabelAssignmentType](../sensitivitylabelassignmenttype/) | The value to set. |
### getSiteId() {#getSiteId--}
```javascript
getSiteId() : string;
```
### setSiteId(string) {#setSiteId-string-}
```javascript
setSiteId(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getContentMarkType() {#getContentMarkType--}
```javascript
getContentMarkType() : SensitivityLabelMarkType;
```
**Returns**
[SensitivityLabelMarkType](../sensitivitylabelmarktype/)
### setContentMarkType(SensitivityLabelMarkType) {#setContentMarkType-sensitivitylabelmarktype-}
```javascript
setContentMarkType(value: SensitivityLabelMarkType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SensitivityLabelMarkType](../sensitivitylabelmarktype/) | The value to set. |
### isRemoved() {#isRemoved--}
```javascript
isRemoved() : boolean;
```
### setIsRemoved(boolean) {#setIsRemoved-boolean-}
```javascript
setIsRemoved(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
