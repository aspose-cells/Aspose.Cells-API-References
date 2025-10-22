##DeleteOptions
Represents the setting of deleting rowscolumns.
## DeleteOptions class
Represents the setting of deleting rows/columns.
```javascript
class DeleteOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [updateReference](#updateReference--)| boolean | Indicates if update references in other worksheets. |
| [formulaChangeMonitor](#formulaChangeMonitor--)| AbstractFormulaChangeMonitor | Gets/sets the monitor for tracking changes caused by the deletion. |
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
