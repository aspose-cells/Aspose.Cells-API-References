##DeleteOptions
Represents the setting of deleting rowscolumns.
## DeleteOptions class
Represents the setting of deleting rows/columns.
```javascript
class DeleteOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [updateReference](#updateReference--)| boolean | Indicates if update references in other worksheets. |
| [formulaChangeMonitor](#formulaChangeMonitor--)| AbstractFormulaChangeMonitor | Gets/sets the monitor for tracking changes caused by the deletion. |
## Methods
| Method | Description |
| --- | --- |
| [getUpdateReference()](#getUpdateReference--)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### updateReference {#updateReference--}
Indicates if update references in other worksheets.
```javascript
updateReference : boolean;
```
### formulaChangeMonitor {#formulaChangeMonitor--}
Gets/sets the monitor for tracking changes caused by the deletion.
```javascript
formulaChangeMonitor : AbstractFormulaChangeMonitor;
```
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
