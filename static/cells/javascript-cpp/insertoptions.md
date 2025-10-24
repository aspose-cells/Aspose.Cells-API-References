##InsertOptions
Represents the options of inserting.
## InsertOptions class
Represents the options of inserting.
```javascript
class InsertOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [copyFormatType](#copyFormatType--)| CopyFormatType |  |
| [updateReference](#updateReference--)| boolean | Indicates if references in other worksheets will be updated. |
| [formulaChangeMonitor](#formulaChangeMonitor--)| AbstractFormulaChangeMonitor | Gets/sets the monitor for tracking changes caused by the insertion. |
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
