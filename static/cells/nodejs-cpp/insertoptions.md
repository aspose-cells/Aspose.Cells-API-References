##InsertOptions
Represents the options of inserting.
## InsertOptions class
Represents the options of inserting.
```javascript
class InsertOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [copyFormatType](#copyFormatType--)| CopyFormatType |  |
| [updateReference](#updateReference--)| boolean | Indicates if references in other worksheets will be updated. |
| [formulaChangeMonitor](#formulaChangeMonitor--)| AbstractFormulaChangeMonitor | Gets/sets the monitor for tracking changes caused by the insertion. |
## Methods
| Method | Description |
| --- | --- |
| [getCopyFormatType()](#getCopyFormatType--)| <b>@deprecated.</b> Please use the 'copyFormatType' property instead. |
| [setCopyFormatType(CopyFormatType)](#setCopyFormatType-copyformattype-)| <b>@deprecated.</b> Please use the 'copyFormatType' property instead. |
| [getUpdateReference()](#getUpdateReference--)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if references in other worksheets will be updated. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if references in other worksheets will be updated. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the insertion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the insertion. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### copyFormatType {#copyFormatType--}
```javascript
copyFormatType : CopyFormatType;
```
### updateReference {#updateReference--}
Indicates if references in other worksheets will be updated.
```javascript
updateReference : boolean;
```
### formulaChangeMonitor {#formulaChangeMonitor--}
Gets/sets the monitor for tracking changes caused by the insertion.
```javascript
formulaChangeMonitor : AbstractFormulaChangeMonitor;
```
### getCopyFormatType() {#getCopyFormatType--}
```javascript
getCopyFormatType() : CopyFormatType;
```
**Returns**
[CopyFormatType](../copyformattype/)
### setCopyFormatType(CopyFormatType) {#setCopyFormatType-copyformattype-}
```javascript
setCopyFormatType(value: CopyFormatType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CopyFormatType](../copyformattype/) | The value to set. |
### getUpdateReference() {#getUpdateReference--}
```javascript
getUpdateReference() : boolean;
```
### setUpdateReference(boolean) {#setUpdateReference-boolean-}
```javascript
setUpdateReference(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```javascript
getFormulaChangeMonitor() : AbstractFormulaChangeMonitor;
```
**Returns**
[AbstractFormulaChangeMonitor](../abstractformulachangemonitor/)
### setFormulaChangeMonitor(AbstractFormulaChangeMonitor) {#setFormulaChangeMonitor-abstractformulachangemonitor-}
```javascript
setFormulaChangeMonitor(value: AbstractFormulaChangeMonitor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../abstractformulachangemonitor/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
